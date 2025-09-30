# .config
My OS is [Omarchy](https://omarchy.org/)

# Wifi
Default WiFi driver is `rtw89-8852be` which is very buggy, so I use this instead

```bash
yay -S rtw89-dkms-git
echo "blacklist rtw89-8852be" | sudo tee /etc/modprobe.d/rtw89_blacklist.conf
```

# Git
In order to connect my git to GitHub:

```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
cat ~/.ssh/id_ed25519.pub
```
