## Setup: Zsh & OhMyZsh on Debian based distro

*Updating system & Installing basic tools*

    sudo  apt-get update
    sudo apt install curl wget git

*Installing powerline fonts and Zsh*

    sudo apt-get install powerline fonts-powerline
    sudo  apt-get install  zsh

*Confirming Installation & Changing default shell*

    zsh  --version
    whereis  zsh
    chsh -s /bin/zsh

*Installing OhMyZsh*

    git clone [https://github.com/robbyrussell/oh-my-zsh.git](https://github.com/robbyrussell/oh-my-zsh.git) ~/.oh-my-zsh
    cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc
    

*Intalling zsh-autosuggestions & zsh-syntax-highlighting plugins*

    
    git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
    git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting

*Installing & Setting up Spaceship Prompt*

    git clone https://github.com/spaceship-prompt/spaceship-prompt.git "$ZSH_CUSTOM/themes/spaceship-prompt" --depth=1
    ln -s "$ZSH_CUSTOM/themes/spaceship-prompt/spaceship.zsh-theme" "$ZSH_CUSTOM/themes/spaceship.zsh-theme"

*Making changes to zsh resource file*
   
     nano ~/.zshrc
     ZSH_THEME="spaceship"
     plugins=(git zsh-autosuggestions zsh-syntax-highlighting)

 
