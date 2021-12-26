# dotfiles

1. Clone the repo in .dotfiles directory `git clone https://github.com/el1t1st/dotfiles.git`.
2. `cd .dotfiles`
3. `./install.sh`
4. Open new terminal.

If you want to remove an errorneous install, use the './cleanup.sh` script. 

If you encounter an error where the chsh requests a password and doesn't accept a valid password change the `/etc/pam.d/chsh` script as follows:

`auth sufficient pam_shell.so`


