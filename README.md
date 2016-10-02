# es-theme-gbz35
Gameboy Zero 3.5" Theme for EmulationStation

This theme pulls heavily from the Spare and SimpleBigArt themes.  It is optimized for resolutions up to 640x480 on small 4:3 screens (like the 3.5" screens commonly used in Gameboy Zero builds).  It also works on 16:9 screens but you will notice that the background art is stretched when viewing in this aspect.

Installation for PC Users
-----------

You will need to connect the Pi Zero to Wifi.  Then, from another computer on the same WiFi network, SSH in (or use Putty on PCs).  Default password is 'raspberry'.:
```
ssh pi@retropie.local
```

Now modify the permissions on the themes folder so it can be modified using a Windows PC over Wifi.
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
writeable - yes
guest ok - yes
create mask = 0644
directory mask = 0755
force user = pi
```

Ctrl-X, and overwrite the original filename.

Now reboot your Pi.
```
sudo reboot now
```

Once you've rebooted, you should be able to access the themes folder on your RETROPIE machine in Windows through File Explorer.  Copy the contents of this theme into the themes folder.

Restart EmulationStation on your Pi, and you should be able to switch to this theme in the UI Settings.
