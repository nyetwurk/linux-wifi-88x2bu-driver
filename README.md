# Linux 88x2bu driver

Based on TPLinks' T4Uv3_WiFi_linux_v5.3.1_beta linux drivers.

Tested on T4Uv3_WiFi_linux_v5.3.1_beta, Linux 5.7.0

Works in 802.11g/n/ac with hostapd

## Installation

```bash
sudo apt-install build-essential dkms
git clone git@github.com:nyetwurk/linux-wifi-88x2bu-driver.git
sudo cp -a linux-wifi-88x2bu-driver /usr/src/linux-wifi-88x2bu-driver-1.0
cd /usr/src
sudo dkms add -m linux-wifi-88x2bu-driver -v 1.0
sudo dkms build -m linux-wifi-88x2bu-driver -v 1.0
sudo dkms install -m linux-wifi-88x2bu-driver -v 1.0
```
