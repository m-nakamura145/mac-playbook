## mac-playbook
mac用のansible playbook

このplaybookを使う場合は先に以下を行うこと。

## Xcode
1. Xcodeの最新版をinstall
* `$ sudo xcodebuild -license`

## Homebrew
```
$ xcode-select --install
$ ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
$ brew doctor
$ brew update
$ brew install python
$ brew install ansible
```

## Ansible
```
$ HOMEBREW_CASK_OPTS="--appdir=/Applications" ansible-playbook -i hosts -vv localhost.yml
```
