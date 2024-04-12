# vim
So I've been using VIM as my primary editor as far as I can remember. Over the years I got comfortable with plugin choices I always used to improve the editor to fit my needs. Recently, I pumped into *neovim* and though it actually seems to offer nice improvements and it does utilize Lua as backend scripting language instead of the dated vimsScript ... So I've decided to give it a try and this repo will be used to document my customizations for it. Please feel free to copy, use as you see fit within the boundries of the MIT licesnse.    

## Environment 
This will be deployed on a Rocky Linux 9 system with EPEL enabled. 
If EPEL is not enabled in your system you can use 
```bash
$ sudo dnf install epel-release -y
```
## Installing <img src='https://github.com/taibah/vim/assets/3851919/e7ae252d-c113-4a62-ad65-04d5e682e168' width="130" height="30"/>

Now its time to install packages that we need
```bash
$ sudo dnf install neovim neovim-ale neovim-python3 -y
```
after its installed we can test if it working correctly by running it
```bash
$ nvim
```
If things are Good! let's make an alias that would make it our default vim for the current user (this assumes that your shell is set to BASH)
```bash
$ echo 'alias vim=nvim' >> .bashrc
```
To test open a new terminal or simply initiate a new bash session at your current terminal ```bash $ bash``` and call ```bash $ vim``` it should now call NeoVim 
