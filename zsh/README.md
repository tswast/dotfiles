# zsh configuration

To install, first set up Oh My ZSH.

My [favorite ZSH theme is ys](http://blog.ysmood.org/my-ys-terminal-theme/). Set
it in `~/.zshrc`.

```
ZSH_THEME="ys"
```

Then install the customizations.

```
ln -s $(pwd)/tmux.zsh $ZSH_CUSTOM/tmux.zsh
ln -s $(pwd)/vimode.zsh $ZSH_CUSTOM/vimode.zsh
```

