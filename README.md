Dotfiles
========

One day this might be a real dotfiles repo with setup scripts instead of copy and pasting, but today is not that day.

# Homebrew

1. `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

## Misc

1. `brew cask install google-chrome vlc visual-studio-code dropbox private-internet-access`
2. `brew install z`

# Git

1. `brew install git`
2. `ln -h .gitconfig ~/.gitconfig`

# Mac config

Pick whatever you like from https://github.com/mathiasbynens/dotfiles/blob/master/.macos

# Node

1. `curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.5/install.sh | bash`
2. `nvm install node`

# Zsh

1. `brew install zsh`
2. `sudo dscl . -create /Users/$USER UserShell /usr/local/bin/zsh`
3. `sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
4. `ln -h .zshrc ~/.zshrc`

# Tmux

1. `git clone https://github.com/gpakosz/.tmux.git ~/workspace/.tmux`
2. `ln -s -f ~/workspace/.tmux/.tmux.conf ~/.tmux.conf`
3. `ln -h .tmux.conf.local ~/.tmux.conf.local`

# Window management

1. `brew tap crisidev/homebrew-chunkwm`
2. `brew install chunkwm --with-tmp-logging`
3. `ln -h .chunkwmrc ~/.chunkwmrc`
4. After giving access to accessibility tools, chunkwm needs to be restarted: `brew services restart chunkwm`
5. `brew install koekeishiya/formulae/skhd`
6. `ln -h .skhdrc ~/.skhdrc`
6. `brew services start skhd`

# Vim

1. `brew install neovim`
2. `curl -sLf https://spacevim.org/install.sh | bash`
3. `brew tap caskroom/fonts`
4. `brew cask install font-dejavu-sans-mono-for-powerline`

# Docker

1. `brew cask install docker`

# Twitch

1. `brew install streamlink`
2. `brew cask install streamlink-twitch-gui`