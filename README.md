setup:

git clone --separate-git-dir=$HOME/.dotfiles git@github.com:wapno/.dotfiles.git tmpdotfiles
rsync --recursive --verbose --exclude '.git' tmpdotfiles/ $HOME/
rm -r tmpdotfiles
