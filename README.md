# Arch + i3wm 🐧 
This is my Arch config for i3wm.

## Clone this repo 📂
```bash
git clone https://github.com/JEFTEDARIEL123/dotfiles.git
cd dotfiles
```

## Install yay 💾
```bash
sudo pacman -Syu
```
```bash
git clone https://aur.archlinux.org/yay.git
```
```bash
cd yay
```
```bash
makepkg -si
```

## Install packages 💾
```bash
yay -S stow polybar feh alacritty neovim picom rofi maim xclip xdotool
``` 

## Symlink the configs 🖇
```bash
mv ~/.config/i3 ~/.config/old-i3
stow alacritty backgrounds i3 nvim picom polybar prompt rofi
```

## Installing Brew & oh-my-posh 💾
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
```bash
brew install jandedobbeleer/oh-my-posh/oh-my-posh
eval "$(oh-my-posh init bash --config ~/.config/prompt/prompt.omp.json)"
```

## Now install FiraCode Font using 💾
```bash
oh-my-posh font install
```

### Then just press Win+Shift+R to reload i3 🚀
