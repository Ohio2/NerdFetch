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
```yay -S ohio2-nerdfetch```
### Non-arch based distros:
Copy-paste this into your terminal:

```sh
# clone and go into repo
git clone https://github.com/Ohio2/NerdFetch.git
cd NerdFetch/
# install and install manpages 
install -Dm775 ./"Debian and Debian-based"/nerdfetch-ubuntu /usr/bin/nerdfetch-ohio2
install -Dm644 ./doc /usr/local/man/man1/nerdfetch-ohio2.1
gzip /usr/local/man/man1/nerdfetch-ohio2.1
# go back and remove the download
cd ..
rm -rf NerdFetch/
# run
nerdfetch-ohio2
```
### Updating:
```
#remove nerdfetch-ohio2
sudo rm /usr/bin/nerdfetch-ohio2
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
