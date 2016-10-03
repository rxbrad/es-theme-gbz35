# Gameboy Zero 3.5" Theme for EmulationStation

![alt tag](http://i.imgur.com/uQrzXFa.png) ![alt tag](http://i.imgur.com/CM2zs51.png) ![alt tag](http://i.imgur.com/jZWMIdV.png) ![alt tag](http://i.imgur.com/PVOtp8L.png)

This theme pulls heavily from the Spare and SimpleBigArt themes.  It is optimized for resolutions up to 640x480 on small 4:3 screens (like the 3.5" screens commonly used in Gameboy Zero builds).  It also works on 16:9 screens but you will notice that the background art is stretched when viewing in this aspect.

Installation (focused on PC users)
-----------

Use the green button at the top of this Git to download the theme as a ZIP file.

You will need to connect the Pi Zero to Wifi.  Then, from another computer on the same WiFi network, SSH in (use Putty on PCs).  The default password is 'raspberry'.:
```
ssh pi@retropie.local
```

Now modify the permissions on the themes folder so you can copy themes to it over Wifi.
```
sudo chmod 0777 /etc/emulationstation/themes
```

Next, add the themes folder to the list of Samba shares
```
sudo nano /etc/samba/smb.conf
```
Scroll to the end of the file and add the following lines:
```
[themes]
comment = themes
path = "/etc/emulationstation/themes/"
writeable = yes
guest ok = yes
create mask = 0644
directory mask = 0755
force user = pi
```

Hit Ctrl-X, and overwrite the original file.

Once you're out of nano, reboot your Pi.
```
sudo reboot
```

After you've rebooted, you should be able to access the themes folder on your RETROPIE machine in Windows through File Explorer.  If asked for a username and password, the defaults are 'pi' & 'raspberry'.

![alt tag](http://i.imgur.com/B3IsFFW.png)

Open the ZIP that you downloaded here, and copy the 'es-theme-gbz35-master' folder inside that ZIP over to the 'themes' folder on RETROPIE.

![alt tag](http://i.imgur.com/G7YTaMe.png)

The name of the folder you just copied is how it's listed in RetroPie.  Once it's copied over, I like to rename the folder to 'gbz-35', but that's just me.

Restart EmulationStation on your Pi, and you should be able to switch to this theme in the UI Settings.

![alt tag](http://i.imgur.com/vbATdHH.png)
