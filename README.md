# setup

Rosetta 2 (Installed with Monterey)
```bash
/usr/sbin/softwareupdate --install-rosetta --agree-to-license
```

Brew
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> $HOME/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

Command line Tools (or Download Xcode)
```bash
xcode-select --install 
```

Tools
```bash

brew install wget 
brew install grep
brew install git
brew install gh
brew install zsh

# warp or fig with iTerm?
brew install --cask warp
brew install --cask fig
brew install --cask iterm2
brew install --cask visual-studio-code

brew install --cask google-chrome
brew install --cask firefox

brew install --cask slack
brew install --cask notion
brew install --cask discord
brew install --cask zoom
```

ohmyzsh (some issues with warp)
```bash
echo $SHELL
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
cd $HOME/.oh-my-zsh/plugins
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git
echo "source $HOME/.oh-my-zsh/plugins/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> $HOME/.zshrc
```

git
```bash
git config --global init.defaultBranch main
git config --global user.name "Me"
git config --global user.email me@email.com
```

SSH
```bash
ssh-keygen -t ed25519 -C "me@email.com"
pbcopy < ~/.ssh/id_ed25519.pub 
ssh-keygen -t rsa -C "me@email.com"
pbcopy < ~/.ssh/id_rsa.pub
```

# try asdf for both node and ruby

nvm
```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```

Node
```bash
nvm install node
nvm install --lts
nvm use --lts
npm install -g npm
npm install -g yarn
```

Ruby (rbenv or rvm)
```bash
curl -L https://get.rvm.io | bash -s stable
brew install readline
brew install openssl
brew install rbenv 
brew install ruby-build
```

MySQL (with workbench)
```
brew install mysql
brew services start mysql
or 
https://dev.mysql.com/downloads/mysql/
https://dev.mysql.com/downloads/workbench/
```

PostgreSQL
```bash
brew install postgresql
brew services start postgresql
```

Redis
```bash
brew install redis
brew services start redis
```

Mongo
```bash
brew tap mongodb/brew
brew install mongodb-community
brew services start mongodb/brew/mongodb-community
```
