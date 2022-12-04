# Lubuntu LXQT for old people a.k.a customize Lubuntu to look like Windows 10

## Themes:
### Windows 10 Openbox theme

https://www.opendesktop.org/p/1653654

Beállítások - LXQt beállítása - Openbox beállítása - Új téma telepítése - and choose the .obt file

### Lxqt win10 theme

https://store.kde.org/p/1319223/

copy to /usr/share/lxqt/themes/

### Windows 10 icon theme
https://store.kde.org/p/1387736/

copy to /usr/share/icons/

### Windows 10 font 'Segoe UI'
https://askubuntu.com/questions/370890/how-can-i-install-segoe-ui-font

### Similar "Open Sans"

https://ubuntu.pkgs.org/18.04/ubuntu-universe-amd64/fonts-open-sans_1.11-1_all.deb.html

## how to copy if acces denied
1. method: Open 'File Manager' (PCManFM) go to 'Tool' tab and choose 'Open as Administrator'.
2. method: Open 'Terminal' example: cp -r /home/USER/Downloads/Win10 /usr/share/lxqt/themes/


## Install libreoffice with hungarian lang.
Donwload the deb from the official site.
Open terminal 
$ cd LibreOffice_$version_Linux_x86-deb/DEBS/
$ sudo dpkg -i *.deb

## How to change mouse speed
In Terminal write:
xinput --list --short

You will get all the inputs like mouse, keyboard.
Find you mouse device, use its number(e.g.: 11) in the following code:

xinput --list-props 11
This will list all its properties.
Use the number of the "accel" property(e.g.331) in the following code:

xinput --set-prop 11 331 -1
where
11 is the mouse device
331 is the accel property
-1 is the new speed

