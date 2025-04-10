# dependencies

```  
git, wayland, hyprland, waybar, rofi, swayosd-git, konsole, zsh w/oh-my-zsh (https://ohmyz.sh/)
optional vim setup from https://github.com/amix/vimrc.git
```

# first time setup
1)  
```
mkdir $HOME/.dotfiles
git init --bare $HOME/.dotfiles
```
2)  
Put the alias in zshrc/bashrc
```
alias dotfiles='/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME'
```

# adding new config files to track
```
cd $HOME
dotfiles add <config file>  
dotfiles commit -m "<comment>"  
dotfiles push  
```

# setup on new machine
```
git clone --separate-git-dir=$HOME/.dotfiles git@github.com:wapno/.dotfiles.git ~
```
