# Development Environment Setup

## Ubuntu
### Prerequisites:


### Update & Upgrade
Run below commands to update your system.
```sh
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install build-essential
```

### Terminal
Install `terminator` terminal
```sh
sudo apt install terminator
```

### Dotfiles
```sh
git config -f ~/.gitlocal user.email "email@yoursite.com"
git config -f ~/.gitlocal user.name "Name Lastname"

# Clone dotfiles repo
git clone https://github.com/denysdovhan/dotfiles.git $HOME/.dotfiles

# Go to the dotfiles directory
cd $HOME/.dotfiles

# Install dotfiles
./install

# Bootstrap dotfile setup
./scripts/bootstrap

# Don't forget to restart the terminal.
```

### Sdkman
```sh
sudo apt-get install curl
sudo apt-get install unzip
curl -s "https://get.sdkman.io" | bash
```

### Troubleshooting
#### 1. zsh-notify: unsupported environment
Related [issue](https://github.com/black7375/BlaCk-Void-Zsh/issues/8).

Solution:
```sh
sudo apt-get install xdotool wmctrl
```
