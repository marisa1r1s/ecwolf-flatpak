# ecwolf-flatpak
ECWolf, as a Flatpak. This setup allowed me to play ECWolf on Bazzite.

## How To Use This Repo

### Install prerequisites (Flatpak Builder, etc.)

1. Install Flathub repository (if not already installed)
```sh
flatpak remote-add --if-not-exists --user flathub https://dl.flathub.org/repo/flathub.flatpakrepo
```
2. Install Flatpak/Flathub Builder from Flathub
```sh
flatpak install flathub org.flatpak.Builder
```
   
### Build Flatpak

1. Run this command to build the Flatpak
```sh
flatpak run --command=flathub-build org.flatpak.Builder --install net.maniacsvault.ECWolf.yml
```

### Set-up and run!

1. Put your data files (e.g. Wolf3D *.WL6 files, Spear of Destiny *.SOD files, etc.) in the following directory:
```
~/.var/app/net.maniacsvault.ECWolf/data/ecwolf/
```
2. Run the ecwolf Flatpak:
```sh
flatpak run net.maniacsvault.ECWolf
```

## Credits

ECWolf SVG icon sourced from:
```
https://github.com/Jaffacakelover/emulator-icons-svg/
```

ECWolf 256x256 PNG icon sourced from:
```
https://www.steamgriddb.com/icon/23050
```
