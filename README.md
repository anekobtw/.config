# .config
My OS is [Omarchy](https://omarchy.org/)

# Wifi
Default WiFi driver is `rtw89-8852be` which is very buggy, so I use this instead

```
yay -S rtw89-dkms-git
echo "blacklist rtw89-8852be" | sudo tee /etc/modprobe.d/rtw89_blacklist.conf
```
