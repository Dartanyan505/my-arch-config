# My Arch Config

![image](https://github.com/user-attachments/assets/2023e64a-239a-4966-b2c9-a76aeb153170)

I was tired of losing all of my configs every time I break my OS.

First things first, I install arch using [arch install](https://wiki.archlinux.org/title/Archinstall), so most of the packages are installed automatically. We will remove some of them and install others.

## Features of config
+ **OS**     -  Arch
+ **WM**     -  Hyprland
+ **Grub**   -  [patato's grub theme](https://github.com/Patato777/dotfiles/tree/main/grub)
+ **File Manager**   -  Thunar

## Packages to Install
+ **neofetch**            -  Without neofetch, linux is not linux.
+ **sof-firmware**        -  I don't exacly know why but without this package sound devices doesn't get detected.
+ **brightnessctl 🌞**    -  This one helps manage laptop's screen brigtness.
+ **blueman 🔷**          -  GUI to manage bluetooth.
+ **pavucontrol 🔊**      -  GUI to manage sound settings.
+ **grub-customizer**     -  To use customize GRUB.
+ **xorg-xhost**          -  This will fix grub-customizer gui problem.
+ **plymounth**           -  To create a graphical boot process.

This command can be copy-pasted into the terminal to install all the packages: <br>

``` 
sudo pacman -S sof-firmware brightnessctl blueman pavucontrol grub-customizer thunar plymounth
```

Also use this command to uninstall unnecessary packages.
``` 
sudo pacman -Rs dolphin
```

## GRUB Customization
I really like [patato's grub theme](https://github.com/Patato777/dotfiles/tree/main/grub)! 🎮
![image](https://github.com/user-attachments/assets/5011aef3-8219-47d0-8c3d-4acd9154c6e6)


If you get the error `` Gtk-WARNING **: 20:26:54.736: cannot open display: :0 `` when trying to run GRUB customizer, install xorg-xhost package and run the command bellow.
```
xhost si:localuser:root
```
This should fix it. 🔧

Replace the themes folder of GRUB customizer and set the theme.

## Boot Customization
