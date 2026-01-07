# ecwolf-flatpak
ECWolf, as a Flatpak. This setup allowed me to play ECWolf on Bazzite.

## How To Use This Repo

### Install prerequisites (flatpak-builder, etc.)

1. Install Flathub repository (if not already installed)
   ```sh
   flatpak remote-add --if-not-exists --user flathub https://dl.flathub.org/repo/flathub.flatpakrepo
   ```
2. Install Flatpak/Flathub builder from Flathub
   ```sh
   flatpak install flathub org.flatpak.Builder
   ```
   
### Build Flatpak

1. Run this command to build the Flatpak
  ```sh
  flatpak run --command=flathub-build org.flatpak.Builder --install net.maniacsvault.ecwolf.yml
  ```

### Set-up and run!

1. Put your data files (e.g. Wolf3D *.WL6 files, Spear of Destiny *.SOD files, etc.) in the following directory:
   ```
   ~/.var/app/net.maniacsvault.ecwolf/data/
   ```
2. Run the ecwolf Flatpak:
   ```sh
   flatpak run net.maniacsvault.ecwolf
   ```
