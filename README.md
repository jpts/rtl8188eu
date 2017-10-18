# RTL8188EU Driver

 * v4.3.0.8 driver (most recent) from [TP-Link](http://www.tp-link.com/us/download/TL-WN722N_V2.html#Driver)
 * patched for 4.x.x kernel

## Notes

 * Known to work on:
   * 4.13.5 kernel (Fedora 26)

 * Know to work with devices:
   * TP-Link TL-WN722N

## Installation
### One-Off
```
cd rtl8188eus-v4.3.0.8
make
insmod 8188eu.ko
```

### DKMS
```
sudo dkms add ./rtl8188EUS-v4.3.0.8
sudo dkms build 8188eu/1.0
sudo dkms install 8188eu/1.0
```
