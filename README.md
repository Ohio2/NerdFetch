# NerdFetch
 A POSIX Linux/macOS fetch script using Nerdfonts

![Screenshot](https://i.imgur.com/rgW5nN1.png)

### Dependencies:

- [Any nerdfonts font](https://www.nerdfonts.com/font-downloads)
- bc (optional, but most systems already have this)
- Pretty much any Linux distro/macOS

### To install and run:
### Arch based distros: (COULD BE USED TO UPDATE ON ARCH-BASED!)
```makepkg -si```
### Or:
```yay -S nerdfetch```
### Non-arch based distros:
Copy-paste this into your terminal:

```sh
# clone and go into repo
git clone https://github.com/ThatOneCalculator/NerdFetch.git
cd NerdFetch/
# install and install manpages 
install -Dm775 ./"Debian and Debian-based"/nerdfetch-ubuntu /usr/bin/nerdfetch
install -Dm644 ./doc /usr/local/man/man1/nerdfetch.1
gzip /usr/local/man/man1/nerdfetch.1
# go back and remove the download
cd ..
rm -rf NerdFetch/
# run
nerdfetch
```
### Updating:
```
#remove nerdfetch
sudo rm /usr/bin/nerdfetch
#Follow To install and run.
```
## Features:
- Terminal Detection
- Shell detection
- Package manager detection?
### OSes supported:
- Ubuntu based Linux (Debi script)
- Arch based Linux (normal script)
- Other (Pengoo script, will not be updated...)
(Logos)


### Known issues:
- No support for BSD package managers/uptime calculations.
- Completely breaks on Android due to the fact that /etc/os_release doesn't exist on Android
- Weird spacing on macOS if you use brew given its complete weirdness
- In [Cool-Retro-Term](https://github.com/Swordfish90/cool-retro-term), the coffee icon shows up as a Chinese character. To fix this, simply change the default font to a NerdFont you installed, or change the existing coffee icon to `nf-fa-coffee` from the [NerdFonts cheet sheet](https://www.nerdfonts.com/cheat-sheet).
