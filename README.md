# What is it?
This is an **official** repo of **SecondOS**(based on ALCI)

# What this repository contains?
This repository contains the official NVIDIA drivers: **nvidia-580xx** and **nvidia-470xx** from AUR and other.

# How to add this repo to my Arch Linux?
Open /etc/pacman.conf by **nano** or other editor and type this at the end: 
```bash
[second-os-repo]
SigLevel = Optional TrustAll
Server = https://github.com/twoerror/second-os-repo/releases/download/db
```
Then, type in terminal:
```bash
sudo pacman -Syy
```
And then you can download packages from this repo! 
For example,
```bash
sudo pacman -S nvidia-470xx-dkms nvidia-470xx-utils lib32-nvidia-470xx-utils
```
>[!TIP]
>Remember about dependencies like ```base-devel``` or ```linux-headers```
