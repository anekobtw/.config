# .config
My OS is [Omarchy](https://omarchy.org/)

The theme I use is `Osaka Jade` (will probably be changed later)

I really love MapleMono font, so:

```bash
yay -S maplemono-nf-unhinted
```

# Wifi
Default WiFi driver is `rtw89-8852be` which is very buggy, so I use this instead

```bash
yay -S rtw89-dkms-git
echo "blacklist rtw89-8852be" | sudo tee /etc/modprobe.d/rtw89_blacklist.conf
```

# Git
In order to connect my git to GitHub:

```bash
git config --global user.email "your_email@example.com"
git config --global user.name "your_name"
ssh-keygen -t ed25519 -C "your_email@example.com"
cat ~/.ssh/id_ed25519.pub
```


# Editor
Usually I would download and configure `nvim` but since `lazyvim` is pre-installed and meets all my requirements, I'm not changing anything

# Packages
Omarchy has a lot of packages pre-installed but I still I always download this

```bash
yay -S telegram-desktop
```

