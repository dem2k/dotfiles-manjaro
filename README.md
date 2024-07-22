````
#
# install programms
#
sudo pacman -S git fzf alacritty lazygit neovim zoxide chezmoi
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
chezmoi init https://github.com/dem2k/dotfiles-manjaro
chezmoi update
````

