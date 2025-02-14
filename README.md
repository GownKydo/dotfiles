# BSPWM and polybar configurations


This repository has been designed with the purpose of being able to set up a light and basic bspwm environment to learn how to start configuring one of your own and be adapted to your needs and tastes.


**Table of content**

* [Installation](#installation)
* [Muanal Installation](#manual-installation)
* [Screenshots](#screenshots)
* [keybinds](#keybinds)


## Installation

First we need to give run permissions to the _install.sh_ file and execute. 

```bash
cd ~/Desktop
git clone https://github.com/GownKydo/dotfiles.git
cd dotfiles
chmod +x install.sh &&./install.sh

```

After this we will execute the file and reboot the system.

> Mover los archivos _.zip_ a la carpeta fonts de tu sistema

## Manual Installation

**Install following software**

* bspwm
* sxhkd
* polybar
* rofi
* i3lock
* amixer
* zsh
* brightnessctl
* feh 
* picom
* neofetch
* cowsay
* ranger
* alacritty
* lolcat
* htop
* flameshot

```bash
bspwm sxhkd polybar rofi i3lock amixer zsh brightnessctl feh picom neofetch cowsay ranger alacritty lolcat htop flameshot

```

Install fonst recommended on this site: [hack nerd fonts](https://www.nerdfonts.com/font-downloads). Download and install the fonts, for change the icons you can do on this site: [nerd fonts cheat sheet](https://www.nerdfonts.com/cheat-sheet)

<br>

## Screenshots

### Desktop

**neofetch, htop, ranger, cowsay with lolcat and nvchad**

![Desktop](/screenshots/desktop.png)

**Brave, obsidian and bat**
![Desktop](/screenshots/desktop2.png)


### Polybar

The blue color in the polybar indicates that the window is occupied by some application, the gray color indicates that it's empty and the pacman indicates in which window we are.

![polybar1](/screenshots/polybar1.png)

![polybar2](/screenshots/polybar2.png)

<br>

## keybinds

### Keysbinds for volume and Brightness

| **keybinds** | Command | **application** | 
|-|-|-|
| XF86MonBrightnessUp | brightnessctl set +10% | Brightness up |
| XF86MonBrightnessDown| brightnessctl set 10%- | Brightness down |
| XF86AudioRaiseVolume| amixer set Master 10%+ | Raises volume | 
| XF86AudioLowerVolume | amixer set Master 10%- | Lowers volume |
| XF86AudioMute | amixer -D pulse set Master 1+ toggle | Mute



### Launch applications

| **keybinds**  | **application** | 
|-|-|
| super + d | rofi |
| super + w | close window |
| super + enter | terminal alacritty | 
| super + shift + b | brave-browser |
| super + shift + m | telegram desktop |
| Print | flameshot gui | 
| super + shift + o | obsidian |
| super + shift + v | Visual Studio Code

> Modify the file `.config/sxhkd/sxhkdrc` for add o change shortcuts
