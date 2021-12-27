# Akisa's DWM config

###My setup for DWM, it includes Tokyo Night color scheme by default but you can change that by adding a color scheme to the *themes* folder.

**To make this set up work properly you will need libxft-bgra. Download it from AUR.**
**If there are any conflicts with normal libxft just agree to replace it.**

```bash
$ git clone https://aur.archlinux.org/libxft-bgra.git
$ cd libxft-bgra && makepkg -si
```

## Dependencies
```
ttf-jetbrains-mono
```

## Installation

```bash
$ git clone https://github.com/akisarazbu/dwm
$ cd dwm && sudo make clean install
```

**After doing these steps, put code below into your .xinitrc**
```bash
while true; do
    # Log stderror to a file 
    dwm 2> ~/.dwm.log
    # No error logging
    #dwm >/dev/null 2>&1
done
```
