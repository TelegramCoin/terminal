# terminal

## oh-my-zsh https://github.com/robbyrussell/oh-my-zsh

- `sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
- Install `afowler` theme

## zsh-autosuggestions https://github.com/zsh-users/zsh-autosuggestions

- `git clone git://github.com/zsh-users/zsh-autosuggestions $ZSH_CUSTOM/plugins/zsh-autosuggestions`
- Enable in `.zshrc`

## z https://github.com/robbyrussell/oh-my-zsh/tree/master/plugins/z

- Enable in `.zshrc`

## brew http://brew.sh/

- `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

## rbenv https://github.com/rbenv/rbenv

- `brew install rbenv`
- `rbenv install 2.3.1`
- `rbenv global 2.3.1`
- `rbenv rehash`
- `echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.zshrc`
- Put `eval "$(rbenv init -)"` at bottom of `zshrc`

## cocoapods

- `gem install cocoapods`

### fastlane

- `gem install fastlane`

## carthage

- https://github.com/carthage/carthage

## quicklook

- https://github.com/sindresorhus/quick-look-plugins

`brew cask install qlcolorcode qlstephen qlmarkdown quicklook-json qlprettypatch quicklook-csv betterzipql qlimagesize webpquicklook suspicious-package`

- https://github.com/lexrus/QLSwift

## dotfiles

- https://github.com/mathiasbynens/dotfiles
- https://github.com/thoughtbot/dotfiles

# Softwares

## List

- iTerm
- 1 Password
- Chrome
- Slack
- Evernote
- Monosnap
- Sublime Text
- Calendar 2
- SourceTree
- Flux https://justgetflux.com/
- Atom
- VSCode
- [Background Music](https://github.com/kyleneideck/BackgroundMusic)
- Asset Catalog Creator

## Xcode

- DarkSide

```sh
curl -fsSL https://raw.githubusercontent.com/onmyway133/terminal/master/themes/Xcode/install.sh | sh
```

- Reveal https://revealapp.com/
- Injection https://github.com/johnno1962/InjectionApp

## Sketch

- https://github.com/onmyway133/Sketch-Action
- https://github.com/timuric/Content-generator-sketch-plugin

## Simulator

- https://github.com/hyperoslo/Simulator

## Chrome

- Ghostery
- Tampermonkey
- Adblock
- Personal Blocklist
- Share on Twitter

# Misc

## Github

- https://github.com/onmyway133/fantastic-git#github
- https://github.com/facebook/mention-bot
- http://danger.systems/


## Git

- http://merowing.info/2016/08/setting-up-pre-commit-hook-for-ios/
- https://appventure.me/2016/04/04/prevent-accidental-test-code-commits/
- http://pre-commit.com/
- Hooks

### Hooks

```
git config core.hooksPath /Users/khoa/hooks
```

### gpg2

- https://help.github.com/articles/generating-a-new-gpg-key/
- https://git-scm.com/book/tr/v2/Git-Tools-Signing-Your-Work

```
brew install gpg2
brew install pinentry-mac
git config --global gpg.program gpg2
echo "test" | gpg2 --clearsign
gpg2 --gen-key
gpg2 --list-secret-keys | grep ^sec
gpg2 --armor --export C85BFA6F // add to GitHub
git config --global user.signingkey C85BFA6F
```

Don't need gpg2

```
git config --global commit.gpgsign false
```
