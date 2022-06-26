# Linux for Beginners

- [Linux for Beginners](#linux-for-beginners)
  - [Commands](#commands)
  - [Arch](#arch)
    - [paru-bin](#paru-bin)
    - [Blackarch repos](#blackarch-repos)

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
