# Screenshots
![Screenshot1](https://user-images.githubusercontent.com/103518800/166099314-38ee1c51-2d3f-4ade-b7f7-d7acda3c94dc.png)
## The RAM usage was high because alot of windows open. (normal usage is ~600MB)
![Screenshot2](https://user-images.githubusercontent.com/103518800/166099324-c2839a61-1e7a-48c3-a012-07947d7239c9.png)

## Why would i even install this OS?
If you value your privacy, mental sanity, and your wallet, **klenhaOS** is for you.
This OS gives you complete **POWER**, **FREEDOM** and **PRIVACY** over your device.
Say no to useless hardware eating! Say yes to freedom! Say no to random crashing! Say yes to **klenhaOS!**

# klenhaOS Installation (TBF)
## Before you install (WARNING)
1. you are gonna remove your system by installing different OS on it if you are not partitioning your drive (if you have no expirience about linux), **USE VIRTUAL MACHINES**
2. i do not guarantee that your stuff will work 100%. i am just a poor soul trying to make his own config files. :)
3. if you have any trouble, let me know on matrix channel. #klenha@matrix.org
4. i am **NOT** going to upload ISO files. building ISO files is buggy and mostly didn't work for really well, so i plan on publishing config files instead.
5. **MAKE SURE YOU EDIT THE CONFIG CALLED AUTOSTART (OR .XPROFILE), IT COULD FUCK YOUR MONITOR IF UR NOT 144HZ USER**
6. the xfce version is not the best one, it was my first time doing any sort of shit with xfce theming, the same with I3 but i am happy with I3 more. it also uses less ram and power.
7. if the themes for WMs are not uploaded, don't worry, it will be soon!
8. before you shit talk to me that my config doesn't work, make sure you have all the fonts, make sure you have all the files configured right.

## Known issues
1. (I3 pure arch) some of the steam games may crash on startup, no idea why
2. (I3 pure arch) the PS1 (username@hostname) in terminal could be overwritten, I don't know why is it, and you fix it by not using the green colors, so removing (or commenting) the piece of PS1=... line in ~/.bashrc
3. (I3 pure arch) changing the volume repeatedly will show super high CPU usage, even if its not.


# klenhaOS Pure Arch I3 version installation
## minimal archinstall script with xorg config **(THE ARCHINSTALL COULD CHANGE, WORK IN PROGRESS!!!!)**
-additional packages- firefox, nano, kate, neofetch, alacritty, i3-wm, i3status, element-desktop thunar, p7zip, vlc(type it out without . signs)
-NEEDED AUR PACKAGES- ly lightshot
-add this line into ~/.xinitrc using nano 
`nano .xinitrc`
`exec i3`
## ADD YOUR USER INTO WHEEL GROUP
`usermod -a -G wheel username`
`su`
`nano /etc/sudoers`
UNCOMMENT %wheel ALL=(ALL:ALL) ALL 
## ENTER I3 
`startx`
## INSTALL .BASHRC
## INSTALL ALACRITTY.YML INTO ~/.config/alacritty/alacritty.yml (create if not found)
## INSTALL I3 THEME (~/.config/i3/config) WITH I3BAR
if you are using a virtual machine, make sure you configure i3bar to show on your real output.
`cd .config/i3/`
`kate config`
search for "HDMI-0" and replace it with your output.
if you are not sure which output you are using, check out
`xrandr`
the output will look crazy, but you can see *** connected in the first lines of it.
most of the time it is probably Virtual-1.


6. i3 theme with i3bar
7. custom terminal and bashrc
8. LY (display manager) config
9. lsb-release, neofetch
10. rofi theme


.
.
.
.
.
.
.
.

## klenhaOS Manjaro XFCE version (ABANDONED)
pre step) preinstall related programs and the base os 
1. bashrc
2. neofetch config
3. lsb release
4. terminal config file
5. xfce theme
6. xfce window theme
7.
