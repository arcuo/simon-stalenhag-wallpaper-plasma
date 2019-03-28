# Simon Stålenhag wallpaper scraper

I made this script for downloading Simon Stålenhag wallpaper from his website and store them locally and apply them as my wallpaper on my Gnome desktop.

Personally i combined this script with a systemd timer so the wallpaper is changed every hour.
## Requirements

python3
Gnome3 desktop or Ubuntu KDE Plasma 5
Systemd

## From this fork

Made original https://github.com/naueramant/simon-stalenhag-wallpaper work with KDE Plasma 5 desktop.

## How to use

This will set the desktop wallpaper to a random image

```sh
python stalenhag.py
```

This will download all images on the website

```sh
python stalenhag.py all
```

This will start or stop the Systemd timer.

```sh
stalenhag timerstart
stalenhag timerstop
```

Manage favorite wallpapers

```sh
stalenhag save
stalenhag list
stalenhag -f

stalenhag clear
```

Get help

```sh
stalenhag -h
stalenhag --help
```

## systemd

An example of a systemd timer and service can be found in the systemd folder.

## Install

For easy installation and removal you can use the scripts

```sh
# Install (prompts for root)
./install.sh

# Uninstall (prompts for root)
./uninstall.sh
```
