# 环境设置 Environment Setup
在[官网](https://www.python.org/downloads/)下载相应平台的安装包安装。

macOS 可以通过pyenv安装和管理2.x和3.x版本的Python。
1. 安装brew
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
2. 安装pyenv
```
brew install pyenv
```
3. 安装python
```
pyenv install 2.7.15 && pyenv install 3.7.0
```
4. 设置默认版本(此处设置的是3.7.0，可根据需要随时切换)
```
pyenv global 3.7.0
```
