````
#
# install programms
#
sudo pacman -S --needed git fzf alacritty lazygit neovim zoxide chezmoi mc bat
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k

chezmoi init https://github.com/dem2k/dotfiles-manjaro --apply
#chezmoi update

git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --global pull.rebase false # Merge

#
````

