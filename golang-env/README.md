# Golang Setup

## Vim Plugins

Please refer the [link](https://github.com/junegunn/vim-plug)

```bash
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
 ```
 
 Following should be the contents of ~/.vimrc
 
 ```bash
 call plug#begin('~/.vim/plugged')

" Using a tagged release; wildcard allowed (requires git 1.9.2 or above)
Plug 'fatih/vim-go'


call plug#end()

filetype off 
filetype plugin indent on

set noswapfile 
set number 
set tabstop=2
set shiftwidth=2
set expandtab
set sts=2

set autoindent
set incsearch
set hlsearch
set showcmd
set autowrite
set ignorecase
set backspace=indent,eol,start
set ai "Auto indent
set si "Smart indent
set wrap "Wrap lines
let mapleader=","
if has("autocmd")
  autocmd FileType go set ts=2 sw=2 sts=2 noet nolist autowrite
endif

syntax on

retab
```
