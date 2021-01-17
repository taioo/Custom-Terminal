Custom Terminal
--------

<img src="terminal.png"/>

## Install packages

#### [font-nerd-font](https://github.com/ryanoasis/nerd-fonts#option-3-install-script)
( via [homebrew](https://brew.sh) )
```
brew tap homebrew/cask-fonts && brew cask install font-hack-nerd-font
```

#### [oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh)
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

 #### [powerlevel10k](https://github.com/romkatv/powerlevel10k) in oh-my-zsh
( Powerlevel10k understands all [Powerlevel9k](https://github.com/Powerlevel9k/powerlevel9k) configuration parameters )
```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/themes/powerlevel10k
```
#### [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting) in oh-my-zsh
```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ~/.oh-my-zsh/custom/plugins/zsh-syntax-highlighting
```

#### [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions) in oh-my-zsh
```
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
```


#### Update powerlevel10k & zsh-syntax-highlighting
```
git -C ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k pull &&
git -C ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting pull
```


</br>
</br>
</br>

## Edit zsh profile file

#### To open zsh profile
```
open .zshrc
```

#### Change theme
```
ZSH_THEME="powerlevel10k/powerlevel10k"
```
#### Edit plugins
```
plugins=(
git
osx
zsh-syntax-highlighting
zsh-autosuggestions
)
```
### customise Powerlevel9/10k

run in terminal
```
p10k configure
```
or
```
open ~/.p10k.zsh
```



</br>


### Set terminal font to "Hack Nerd Font"

## <center>Have fun</center>

</br>
</br>
</br>
</br>

##  VS Code settings
```
{
"terminal.integrated.fontFamily": "Hack Nerd Font",
}
```
