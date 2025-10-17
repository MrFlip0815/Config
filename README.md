# dotfiles config for nvim tmux and more

## Requirements

### Git

```
sudo apt-get install git
```

### Homebrew

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### Neovim

Make sure version > 0.10.x
```
brew install neovim
```

or

```
sudo apt-get install neovim
```

### Tmux

```
sudo apt-get install tmux
```

to fix tmux window pane renaming make sure to check out the catppuccin options file 
https://www.reddit.com/r/tmux/comments/1conb7k/having_issue_with_window_titles/

### Oh My Posh

```
brew install oh-my-posh
```

### Stow

```
sudo apt-get install stow
```

### Nerd Font

```
download at https://www.jetbrains.com/lp/mono/
``` 

### RipGrep (Telescope)
```
sudo apt-get instral ripgrep
´´´


## Installation

```
cd ~
mkdir dotfiles && cd dotfiles
git clone https://github.com/MrFlip0815/Config.git
cp -rp Config/. ~/dotfiles
rm -rf Config
stow . --adopt
git restore .
```

# zsh plugins (optional)

```
mkdir ~/testplugin/
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git /testplugin/zsh-syntax-highlighting/
git clone https://github.com/zsh-users/zsh-autosuggestions ./testplugin/zsh-autosuggestions
```

# Tmux/TPM
```
git clone https://github.com/tmux-plugins/tpm ~/.config/tmux/plugins/tpm
modify tmux config in '~/dotfiles/.config/tmux/tmux.conf' for tpm to load properly '~/dotfiles/.config/tmux/plugins/tpm/tpm
´´´

## Video and Guides

https://www.youtube.com/watch?v=y6XCebnB9gs
