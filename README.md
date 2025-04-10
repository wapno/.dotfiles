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
