# Linux for Beginners

- [Linux for Beginners](#linux-for-beginners)
  - [Commands](#commands)
  - [Tools](#tools)
  - [Terminal utilities](#terminal-utilities)
  - [Arch](#arch)
    - [paru-bin](#paru-bin)
    - [Blackarch repos](#blackarch-repos)
    - [AwesomeWM & picom](#awesomewm--picom)
    - [pulseaudio & pactl](#pulseaudio--pactl)

## Commands

* `cfdisk`: Partitioning tool w/GUI.
* `lsblk`: List block devices.
* `neofetch`: Get system info.
* `sudo systemctl start NetworkManager.service`: Start network manager.
* `sudo systemctl enable NetworkManager`: Enable network manager.
* `sudo systemctl start wpa_supplicant.service`: Start wpa_supplicant.
* `sudo systemctl enable wpa_supplicant.service`: Start wpa_supplicant.
* `ps aux`: List processes.
* `kill -9 <pid>`: Kill process.

## Tools

* [rofi](https://github.com/davatorium/rofi)
* [Font awesome](https://www.onea.be/wp-content/themes/agile-child/font-awesome-4.3.0/css/)
* [streetturtle/awesome-wm-widgets: Widgets for Awesome Window Manager (github.com)](https://github.com/streetturtle/awesome-wm-widgets)
* [Arch Linux - lxappearance-gtk3 0.6.3-4 (x86_64)](https://archlinux.org/packages/community/x86_64/lxappearance-gtk3/)
    - Place themes on /usr/share/themes
    - [papirus-icon-theme](https://github.com/PapirusDevelopmentTeam/papirus-icon-theme)
* [GTK - ArchWiki (archlinux.org)](https://wiki.archlinux.org/title/GTK)
* zsh
    - `sudo su` & `ln -s -f /home/<user>/.zshrc /root/.zshrc`
* xclip
* pulseaudio
  * pactl

## Terminal utilities

* scrub
* lsd
* bat
* bspwm

## Arch

I like to keep the following stuff in `mkdir -p Desktop/<user>/repos`.

### paru-bin

```
git clone https://aur.archlinux.org/paru-bin.git
cd paru-bin
makepkg -si
```

### Blackarch repos

```
mkdir blackarch
curl -O https://blackarch.org/strap.sh
chmod +x strap.sh
sudo su
./strap.sh
pacman -Sy
```

### AwesomeWM & picom

* `xgrep | grep -i class`: Search for a window.

### pulseaudio & pactl

* volume up: `pactl set-sink-volume 0 +5%`
* volume down: `pactl set-sink-volume 0 -5%`
* mute: `pactl set-sink-mute 0 false`
* unmute: `pactl set-sink-mute 0 true`
