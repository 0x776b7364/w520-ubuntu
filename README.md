# The W520 Ubuntu Project

This project aims to document how my custom Ubuntu 18.04 LTS installation can be performed on my Thinkpad W520.

## Considerations

Document all relevant hardware

Document all use-cases with the OS

Stick to GNOME 3, or Xfce, or Xfce-bundled (i.e. Xubuntu)?

Configuring a preseed file, and access it over ftp/http

Post-install scripts

Field-testing in virtualbox before testing on bare-metal

Candidate ISOs: 16.04.3/17.10 mini

Default python version per distro:
- 16.04: 3.5.1
- 17.10: 2.7.14
- 18.04: 3.6.3?

## URLs

https://ubuntuforums.org/showthread.php?t=2361552

https://www.youtube.com/watch?v=klPtcdle_XQ

https://askubuntu.com/questions/122505/how-do-i-create-a-completely-unattended-install-of-ubuntu/122506#122506

https://unix.stackexchange.com/questions/139814/what-values-from-debconf-get-selections-should-not-be-preseeded

https://serverfault.com/questions/143296/how-to-get-http-preseed-to-work-correctly-on-ubuntu-10-04-lts-lucid

https://www.lifewire.com/ubuntu-15-04-vs-xubuntu-15-04-2201174

https://xubuntu.org/news/introducing-xubuntu-core/

https://askubuntu.com/questions/96641/xubuntu-desktop-minimal-installation

https://askubuntu.com/questions/396611/difference-between-lubuntu-mini-core-and-lubuntu-mini-desktop

## Commands

```bash
apt list --installed
grep " installed" /var/log/dpkg.log*
lshw
lsusb
debconf-get-selections --installer
debconf-get-selections
pkginstalls.sh
df -h
```

## Tasksel

TBA

## Current hardware

Commands are executed as root on Ubuntu 16.04.3 LTS.

[lshw](native-lshw-16.04.3.txt)

[lsusb](native-lsusb-16.04.3.txt)

```
4270-CTO
Processor: Intel Core i7-2760QM Processor (2.40 GHz, 6MB L3)
Display type: 15.6″ FHD (1920 x 1080) LED Backlit Anti-Glare Display, Mobile Broadband Ready
System graphics: NVIDIA Quadro 1000M Graphics with 2GB DDR3 Memory
Total memory: 4x 4 GB DDR3 – 1333MHz (total of 16 GB)
Hard drive: Intel 40 GB SSD SATA
Secondary hard drive: Ultrabay with 750GB WD Scorpio Blue 5400rpm
Bluetooth: Broadcam Bluetooth
Integrated WiFi wireless LAN adapters: Intel Centrino Advanced-N 6205 (2×2 AGN)
```
