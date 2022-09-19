# raspihats

Raspihats integration for Home Assistant extracted from Home Assistant 2022.3.8.

[Home Assistant Core 2022.3.8](https://github.com/home-assistant/core/tree/2022.3.8)

[Last Working Raspihats Integration](https://github.com/home-assistant/core/tree/2022.3.8/homeassistant/components/raspihats)


## Raspihats Setup (Arch Linux on Raspberry Pi 4)

```
sudo pacman -S i2c-tools
```
```
# /boot/config.txt

dtparam=i2c_arm=on
```
```
# /etc/modules-load.d/raspberrypi.conf

i2c-dev
```
```
# ha - home assistant config folder
me="$(whoami)"
cd /home/$me/ha/custom_components
git clone https://github.com/pelemarse/raspihats
```
