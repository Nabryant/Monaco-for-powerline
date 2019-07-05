Patched Monaco Font for airline or powerline 
=============================================

Monaco font for airline or powerline vim plugin. Which is tested on gnome terminal in Ubuntu 14.04 LTS.

INSTALL
=======

- Clone or copy current files under your prefered folder
- Open terminal and change to the font directory where you downloaded files
```bash
cd /path/to/directory/which/contains/downloaded/files/font
```
- Move **Ubuntu Mono derivative Powerline.ttf** to your home folder _~/.fonts_. If .fonts direcory does not exists create it (mkdir  ~/.fonts)
```bash
mkdir ~/.fonts
mv Ubuntu\ Mono\ derivative\ Powerline.ttf ~/.fonts
```
- Change to config directory and move **10-powerline-symbols.conf** to *~/.config/fontconfig/conf.d/*. If folders does not exists create them
```bash
mv 10-powerline-symbols.conf ~/.config/fontconfig/conf.d/
```
- Execute following in terminal in order to update font cache and close all terminal windows.
```bash
sudo fc-cache
```
- Open gnome terminal and select __Monaco for Powerline__ in terminal configuration window 
- Open ~/.vimrc in vim and add **let g:airline_powerline_fonts = 1** for enabling powerline fonts in airline
```bash
vim ~/.vimrc
let g:airline_powerline_fonts = 1
```
- Quit from vim and open again. Now you can see powerline symbols in your airline theme.

P.S.: I did not use powerline so I did not tested but it works in airline.
If you wondering why font name **Ubuntu Mono derivative Powerline.ttf** read [here](https://github.com/Lokaltog/powerline-fonts/pull/37)
