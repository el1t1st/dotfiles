# Portable Development Environment

Optimized for Debian bookworm, with support for Boox Mira and Boox Note Air 2.

- zsh (kitty is available, but being downgraded)
- nvim
- haskell, lua, bash, sql, markdown, yaml, ocaml
- support for Chinese (run ibus-setup to set the entry panel)

## Installation Workflow

1. Change the `/etc/pam.d/chsh` file as follows:
   `auth sufficient pam_shell.so`
2. Add user to sudoers, so you can run sudo commands:
   `su -`
   `usermod -a -G sudo alex`
   Add `username ALL=(ALL:ALL) ALL` to /etc/sudoers file.
3. Install git `sudo apt-get install git`
4. Clone the repo in .dotfiles directory `git clone https://github.com/el1t1st/dotfiles.git ~/.dotfiles`.
5. `cd .dotfiles`
6. `./install.sh`

Note: Only works for one user on a debian machine, since nix can't easily handle multiple users on one machine.

# Post-install Neovim

1. Run `:PackerSync` or `:PackerInstall`. This will install the needed packages.

# Remove Workflow

If you want to remove an errorneous install, use the `./cleanup.sh` script. This script not just removes the .local and .config and all dotfiles, but also the /nix directory.

# Haskell

[## Use stack to create and manage haskell projects](https://anvilproject.org/guides/content/creating-links)

1.`stack new my-project` 2.`cd my-project` 3.`stack build` 4.`stack exec my-project-exe`

## Haskell repl

`stack repl`

## Manage Haskell Toolkit

`ghcup tui1

# Russian

Change the keyboard to ANSI.

# Chinese
