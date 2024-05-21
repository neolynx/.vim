# My vim configuration

Programming in python, cpp, golang, angular led to this configuration.

Thanks also to Timo Furrer ;-)

## Prerequisites
```
sudo apt install cmake python3-dev flake8 exuberant-ctags clang python3-watchdog
```

## Installation

```bash
git clone https://github.com/neolynx/.vim ~/.vim
cd ~/.vim
git submodule update --init --recursive
test -f ~/.vimrc && mv ~/.vimrc ~/.vimrc.bak
ln -s ~/.vim/vimrc ~/.vimrc

# install ycm with clang support
cd pack/programming/start/YouCompleteMe

# if you like C++ completion
python3 install.py --clang-completer

# if you like Rust completion
python3 install.py --rust-completer
```
