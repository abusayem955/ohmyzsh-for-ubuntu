# ohmyzsh-for-ubuntu
Oh My Zsh is an open source, community-driven framework for managing your zsh configuration.

## Setup and configur oh-my-zsh procedure:
**In order for Oh-My-Zsh to work, Zsh must be installed. First update the package repository cache of Ubuntu OS.**
```sh
sudo apt-get update
```
Now install **ZSH** with the following command:
```sh
sudo apt-get install zsh
```
To making ZSH the Default Shell, Firstly it need to find out the path of the ZSH shell with the following command:
```sh 
whereis zsh
```
As we can see from the marked section of the screenshot below, the path of ZSH shell is **/usr/bin/zsh**
Now set ZSH as the default login shell for current user
```sh
sudo usermod -s /usr/bin/zsh $(whoami)
```
**Press the number key 2 and ZSH should create a new ~/.zshrc configuration file with the recommended settings.**
## image
## Installing Oh-My-ZSH:
To install **Oh-My-ZSH** from [githubusercontent](https://github.com/ohmyzsh/ohmyzsh), run the following command:
```sh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
## Installing Powerline, Powerline Fonts and Powerlevel9k Theme for ZSH:
Run the following command to install **Powerline** and **Powerline font**
```sh
sudo apt-get install powerline fonts-powerline
```
Run the following command to install **Powerlevel9k ZSH** theme
```sh
sudo apt-get install zsh-theme-powerlevel9k
```
Now run the following command to enable **Powerlevel9k ZSH** theme.
```sh
echo "source /usr/share/powerlevel9k/powerlevel9k.zsh-theme" >> ~/.zshrc
```
Run the following command to install **ZSH Syntax Highlighting** Plugin
```sh
sudo apt-get install zsh-syntax-highlighting
```
Now run the following command to enable **ZSH Syntax Highlighting** plugin:
```sh
echo "source /usr/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ~/.zshrc
```
**Now open a new terminal and see the terminal.**
