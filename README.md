# dotfiles

To debug vim syntastic, add in .vimrc

```
let g:syntastic_debug=3
```

and `:mes` in vim

# ctags and gotags

http://ctags.sourceforge.net

```
go get -u github.com/jstemmer/gotags
go get -u github.com/golang/lint/golint
go get -u github.com/kisielk/errcheck
go get -u golang.org/x/tools/cmd/goimports
```

# plugins

All plugins need to be placed in the `bundle` folder.

```
git clone --depth=1 https://github.com/fatih/vim-go.git
git clone --depth=1 https://github.com/vim-syntastic/syntastic.git
git clone --depth=1 https://github.com/ervandew/supertab.git
pip install flake8
```
Then inside vim
```
:GoInstallBinaries
```

# non-essential plugins

```
git clone https://github.com/majutsushi/tagbar.git
git clone https://github.com/scrooloose/nerdtree.git
```
# link vimrc

```
ln -s ~/dotfiles/vimrc ~/.vimrc
mv ~/dotfiles/bash/* ~/
```

