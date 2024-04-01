# BSPMWM Rice Dotfiles
Hi **everyone**, i would like to say this is our **first** rice we do and publish, so if it is a bit clean or empty is only for that.

## 1) Installing dependencies and start sddm:
We advice you to start that rice in the xorg tty, and then do that:
### **Installing yay**
```bash
    sudo pacman -S --needed git base-devel
    git clone https://aur.archlinux.org/yay.git
    cd yay
    makepkg -si
```
### **Installing dependencies**
Before you **start** copying, i'd like to say to you if you **first clone** this **repo**, you **have** the **dependencies.md** file that you can write more comfortably and to do that you can:
```bash
    cat dependencies.md
```
Or you can simply **copy** that:
```bash
    yay -S bspwm picom sxhkd cava kitty rofi micro neovim nemo spotify-launcher discord sddm feh waterfox-bin lunar-client zsh-autosuggestions zsh-syntax-highlighting zsh-history-substring-search noto-fonts-emoji ttf-joypixels ttf-twemoji otf-openmoji ttf-twemoji-color ttf-symbola
```
### **Start SDDM**
```bash
    sudo systemctl enable sddm
```

## 2) Clone this repo:
To start using our rice, you have to clone this repo to put our config and dotfiles:
```bash
    git clone https://github.com/sakudicion/bspwm-dotfiles
```

## 3) Change Directory:
Now you have to enter in our directory to copy our file:
```bash
    cd bspwm-dotfiles
```

## 4) Copy our config:
Simply you have to copy paste it in your terminal:
```bash
    cd home/config
    sudo cp * ~/.config/
    cd ../Wallpaper
    mkdir ~/Wallpaper
    cp * ~/Wallpaper
    cd ..
    sudo mv zshrc .zshrc
    cp .zshrc ~/
    cd ..
    cd file\ system
    cp bin/sysfetch /bin/
    sudo chmod +x /bin/sysfetch
    cd ..
    cd usr/share/fonts
    cp * /usr/share/fonts
    cd
```

## 5) Now you can reboot
```bash
    reboot
```
