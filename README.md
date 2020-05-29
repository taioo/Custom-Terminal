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
zsh-syntax-highlighting
)
```
#### customise Powerlevel9/10k

#### Paste this example config before "source $ZSH/oh-my-zsh.sh"
```
# Customise the Powerlevel9k prompts

POWERLEVEL9K_LEFT_PROMPT_ELEMENTS=(

  root_indicator 
  os_icon 
  dir 
  vcs 

  )

POWERLEVEL9K_RIGHT_PROMPT_ELEMENTS=(

virtualenv
anaconda
pyenv
nodeenv
nvm
chruby
rbenv
rspec_stats
rvm
aws_eb_env
docker_machine

)

POWERLEVEL9K_ROOT_ICON="sudo"

POWERLEVEL9K_OS_ICON_BACKGROUND="white"
POWERLEVEL9K_OS_ICON_FOREGROUND="black"

# icon start with '\u....'
#POWERLEVEL9K_LEFT_SEGMENT_SEPARATOR='\ue0c0'
#POWERLEVEL9K_RIGHT_SEGMENT_SEPARATOR='\uE0B6'


POWERLEVEL9K_PROMPT_ON_NEWLINE=true
POWERLEVEL9K_STATUS_VERBOSE=false

POWERLEVEL9K_MULTILINE_FIRST_PROMPT_PREFIX=""
POWERLEVEL9K_MULTILINE_LAST_PROMPT_PREFIX=""

# Add the custom apple icon prompt segment
# POWERLEVEL9K_CUSTOM_APPLELOGO="echo -n $'\ufc23'"

# Load Nerd Fonts with Powerlevel9k theme for Zsh
POWERLEVEL9K_MODE='nerdfont-complete'

```

#### OR run in terminal
```
p10k configure
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
