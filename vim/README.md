# Vim configuration

This adds some handy vim plugins as [git submodules][submodule], so if you
didn't clone recursively, initialize the submodules with the commands:

```
git submodule init
git submodule update
```

Then, install [vim-pathogen][pathogen] to `~/.vim/autoload/pathogen.vim`.

```
cd ~/src
git clone https://github.com/tpope/vim-pathogen.git
mkdir -p ~/.vim/autoload
ln -s "${HOME}/src/vim-pathogen/autoload/pathogen.vim" ~/.vim/autoload/pathogen.vim
```

Need to add to the .vimrc:

```
execute pathogen#infect()
```

Now, can link to bundle directory.

```
ln -s "${HOME}/src/dotfiles/vim/bundle" ~/.vim/bundle
```

[pathogen]: https://github.com/tpope/vim-pathogen
[submodule]: https://git-scm.com/book/en/v2/Git-Tools-Submodules

## Adding new plugins

Add new plugins to the `vim/bundle` directory using submodules.

```
cd ~/dotfiles/vim/bundle
git submodule add https://github.com/tpope/vim-sensible.git
```

