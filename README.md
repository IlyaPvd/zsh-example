sudo apt install zsh

sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)”


git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k

echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc


git clone --depth=1 https://github.com/romkatv/nerd-fonts.git


cd nerd-fonts


./install.sh JetBrainsMono

reboot


git clone https://github.com/zsh-users/zsh-syntax-highlighting.git

${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting


plugins=( zsh-syntax-highlighting)


source ~/.oh-my-zsh/zshrc