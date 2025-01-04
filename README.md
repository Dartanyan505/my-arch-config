# My Hayprland Config

![image](https://github.com/user-attachments/assets/d82795c9-ce33-4d07-a05e-d0df9f5f8aad)

I was tired of losing all of my configs every time I break my OS.

## Features of config
+ **OS**     -  arch
+ **Grub**   -  [patato's grub theme](https://github.com/Patato777/dotfiles/tree/main/grub)

## Packages to Install
+ **sof-firmware**        -  I don't exacly know why but without this package sound devices doesn't get detected.
+ **brightnessctl 🌞**    -  This one helps manage laptop's screen brigtness.
+ **blueman 🔷**          -  GUI to manage bluetooth.
+ **pavucontrol 🔊**      -  GUI to manage sound settings.
+ **grub-customizer**     -  To use customize GRUB

This code can be copy-pasted into the terminal to install all the packages: <br>

``` 
sudo pacman -S sof-firmware brightnessctl blueman pavucontrol grub-customizer
```

## GRUB Customization
I really like [patato's grub theme](https://github.com/Patato777/dotfiles/tree/main/grub)!
![image](https://github.com/user-attachments/assets/5011aef3-8219-47d0-8c3d-4acd9154c6e6)


If you get the error `` Gtk-WARNING **: 20:26:54.736: cannot open display: :0 ``, install xorg-xhost package and run the command bellow.
```
xhost si:localuser:root
 ```
