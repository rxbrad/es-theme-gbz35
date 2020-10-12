# Gameboy Zero 3.5" Theme for EmulationStation (OpenDingux RG350 / RG280 Version)

*This is a stripped-down version of the GBZ35  theme, which is compatible with EmulationStation 2.0.0-RC1, which is commonly used on OpenDingux devices.*

[Click here for alternative Dark version of this theme (RG350/RG280 variant)](https://github.com/rxbrad/es-theme-gbz35-dark/tree/RG350_RG280)

![System Select Screen](https://i.imgur.com/iFvnFOJ.png) ![Detailed Game List](https://i.imgur.com/tTtp6dk.png) ![Basic Game List](https://i.imgur.com/Aa0SH5f.png)

This theme pulls heavily from the [Carbon](https://github.com/RetroPie/es-theme-carbon) (controller & system vector art), [Spare](https://github.com/mattrixk/es-theme-spare) (preliminary layout), and [SimpleBigArt](https://github.com/robertybob/es-theme-simplebigart) (preliminary background art) themes.  It is optimized for resolutions up to 640x480 on small 4:3 screens (like the 3.5" screen on the Anbernic RG-350).  It also works on 16:9 screens but you will notice that the background art is stretched when viewing in this aspect.

Changelog
-----------

- Update Oct 12, 2020: Replaced ES 2.0.0-RC1 incompatible SVG logos with alternate versions.
- Update Oct 9, 2020: Replaced garbled SNES logo. Changed Basic gamelist text to left-aligned, since ES 2.0.0-RC1 cannot gracefully handle centered text with some fonts.  Tweaked gamelist text sizes for optimal display.  Removed unsupported Child-Friendly code.
- Update June 8, 2020: **New RG350/RG280 Branch:** Uses July 24, 2017 build, and adds all systems added to current date
- Update Jul 21, 2017: Added carousel theming
- Update Jul 20, 2017: Added MAME variants; folder highlighting in gamelist; prepend folder name with § (Alt-0167) to add a folder icon (need to start folder name with a space to move to top of list)
- Update #3 - Jul 18, 2017: Fixed clipping at the bottom of the gamelist at certain resolutions
- Update #2 - Jul 18, 2017: Added c64, colecovision, intellivision, kodi, & ti99
- Update Jul 18, 2017: Added favorite, all games, recently played and custom-collections functionality
- Update Jul 17, 2017: Added support for video previews (be sure you're on the latest version of RetroPie, and note that the Pi Zero apparently struggles with video previews in RetroPie, so you may only want to scrape videos if you have a Pi2 or Pi3 in your GBZ); fixed Retropie menu screen theme
- Update Feb 9, 2017: Added dark theme and Dosbox section to theme
- Update Dec 16, 2016: Added Child-friendly EmulationStation Icon support in the detailed view
- Update Oct 4, 2016: I tweaked the Basic View to show an 8th game on the screen, and colorized the selected game on the list to match the current system's theme.

License
-----------
Creative Commons CC BY-NC-SA - https://creativecommons.org/licenses/by-nc-sa/3.0/

Installation (OpenDingux RG350 / RG280 Version)
-----------

- Install EmulationStation on your unit using one of many guides available online.  [Here is one such guide.](https://retrogamecorps.com/2020/10/07/guide-emulationstation-on-rg350-devices/)
- Download this theme as a ZIP file using the green "Code" button at the top of the page on this GitHub repository.
- Extract the theme folder to the /media/data/local/home/.emulationstation/themes folder on your internal SD card (Windows users can copy over FTP.  Or you can copy the folder to the external SD, and then use Dingux Commander on your unit to transfer the files to the internal SD)
- Choose the theme under the "UI Settings" section of EmulationStation's Start Menu settings screen (you may need to restart ES for the theme to load gracefully after you select it)
![UI Settings Screen](http://i.imgur.com/vbATdHH.png)
