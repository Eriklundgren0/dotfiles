# dotfiles
Customization files used to personalize Linux.

System: Linux Mint 

Theme: Dracula

## Setup and Use instructions

```
git init --bare $HOME/.cfg

alias config='/usr/bin/git --git-dir=$HOME/.cfg/ --work-tree=$HOME'

config config --local status.showUntrackedFiles no

echo "alias config='/usr/bin/git --git-dir=$HOME/.cfg/ --work-tree=$HOME'" >> $HOME/.bashrc
```
### Use of config alias
```
config status

config add .vimrc

config commit -m "Add vimrc"

config add .bashrc

config commit -m "Add bashrc"

config push
```
### Tutorial

https://www.atlassian.com/git/tutorials/dotfiles

