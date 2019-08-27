# myZSH file


#### install zsh
```
brew install zsh
```
#### Open Bash
```
open ~/.bash_profile
```
#### run zsh in Bash
```
exec zsh
```
#### to open zsh profile
```
open .zshrc
```





 
#### install powerlevel9k
First get the homebrew tap
```
brew tap sambadevi/powerlevel9k
```
Then install powerlevel9k via brew
```
brew install powerlevel9k
```


#### install font-hack-nerd-font
First get the homebrew tap
```
brew tap homebrew/cask-fonts
```
Then install font-hack-nerd-font via brew
```
brew cask install font-hack-nerd-font
```

#### install zsh-syntax-highlighting
```
brew install zsh-syntax-highlighting
```

#### copy and paste to zsh profile file
```
# Customise the Powerlevel9k prompts
POWERLEVEL9K_LEFT_PROMPT_ELEMENTS=(root_indicator os_icon dir vcs )
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
kubecontext

)

POWERLEVEL9K_ROOT_ICON="sudo"

POWERLEVEL9K_OS_ICON_BACKGROUND="white"
POWERLEVEL9K_OS_ICON_FOREGROUND="black"

#POWERLEVEL9K_LEFT_SEGMENT_SEPARATOR='\ue0c0'
#POWERLEVEL9K_RIGHT_SEGMENT_SEPARATOR='\uE0B6'


POWERLEVEL9K_PROMPT_ON_NEWLINE=true
POWERLEVEL9K_STATUS_VERBOSE=false

POWERLEVEL9K_MULTILINE_FIRST_PROMPT_PREFIX=""
POWERLEVEL9K_MULTILINE_LAST_PROMPT_PREFIX=""

# Add the custom apple icon prompt segment
POWERLEVEL9K_CUSTOM_APPLELOGO="echo -n $'\ufc23'"

# Load Nerd Fonts with Powerlevel9k theme for Zsh
POWERLEVEL9K_MODE='nerdfont-complete'

source /usr/local/opt/powerlevel9k/powerlevel9k.zsh-theme
source /usr/local/opt/zsh-syntax-highlighting/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
####end
```
#### set terminal font to "Hack Nerd Font"
