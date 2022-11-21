# QCA9377 Wireless driver
Monitor Mode is working but not packet injection.
## Installation of Driver
- git clone https://github.com/amitkrxyz/qca9377
- `sudo cp firmware-5.bin /lib/firmware/ath10k/QCA9377/hw1.0/`
- `sudo rm /lib/firmware/ath10k/QCA9377/hw1.0/firmware-6.bin`
- Reboot or
    - `sudo rmmod ath10k_pci`
    - `sudo modprobe ath10k_pci`
    - `sudo systemctl restart NetworkManager`

## Tested on
| Distribution      | Kernel            | Device |
|-------------------|-------------------|--------|
| Kali Linux 2022.3 | 5.18.0-kali5-amd64| Qualcomm Atheros QCA9377 802.11ac Wireless Network Adapter (rev 31) |