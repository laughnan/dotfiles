# dotfiles

## Bash

Clone the contents of this repo into: ~/dotfiles:

```
git clone git@github.com:laughnan/dotfiles.git ~/dotfiles
```

Add the following to ~/.bash_profile

```
# Loads dotfiles (customize the list below accordingly)
for file in ~/dotfiles/.{base,git-completion}; do
  [ -r "$file" ] && source "$file"
done
unset file
```

## Vim

Create a symbolic link for the vimrc config

```
ln -s ~/dotfiles/.vimrc ~/.vimrc`
```
