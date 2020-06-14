# dmenu - dynamic menu
====================
dmenu is an efficient dynamic menu for X.

Some patches were applied, as always find attached in the `patches` directory.

Do not blame me if it doesnt work suddenly, because some dmenu flags were removed because of patches.

## Requirements
------------
In order to build dmenu you need the Xlib header files.


## Installation
------------
Edit config.mk to match your local setup (dmenu is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install dmenu
(if necessary as root):

    make clean install


## Running dmenu
-------------
Checkout my [dwm build](https://github.com/DragonGhost7/dwm) for how i launch dmenu, and my [scripts](https://github.com/DragonGhost7/dotfiles/tree/master/bin) because some of them use dmenu and are cool *is this self promotion yes it is fight me*.
