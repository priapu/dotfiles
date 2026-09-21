# dotfiles

Plain files, symlinked into place. No manager, no templating.

## Bootstrap on a new machine

```
git clone <remote-url> ~/dotfiles
ln -sf ~/dotfiles/bashrc ~/.bashrc
mkdir -p ~/.config/ghostty
ln -sf ~/dotfiles/ghostty/config.ghostty ~/.config/ghostty/config.ghostty
```

## Adding a new file

Move the real file into this repo, symlink it back, commit:

```
mv ~/.somerc ~/dotfiles/somerc
ln -s ~/dotfiles/somerc ~/.somerc
git add somerc && git commit -m "add somerc"
```
