
## Email:    quinwoodz@gmail.com
## Phone:    704-470-7036


<!---
quinwoods/quinwoods is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

```
# Prompt
autoload -U colors && colors
PS1="%F{cyan}%n%f@%F{green}%3/%f 
"
# Syntax Highlighting
source ~/Software/zsh/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh 
#Auto-complete
autoload -U compinit
zstyle ':completion:*' menu select
zmodload zsh/complist
compinit
_comp_options+=(globdots)
#Syntax Highlighting man pages
man() {
    LESS_TERMCAP_md=$'\e[01;31m' \
    LESS_TERMCAP_me=$'\e[0m' \
    LESS_TERMCAP_us=$'\e[01;32m' \
    LESS_TERMCAP_ue=$'\e[0m' \
    LESS_TERMCAP_so=$'\e[45;93m' \
    LESS_TERMCAP_se=$'\e[0m' \

    command man "$@"
}

export LESS_TERMCAP_mb=$'\e[1;32m'
export LESS_TERMCAP_md=$'\e[1;32m'
export LESS_TERMCAP_me=$'\e[0m'
export LESS_TERMCAP_se=$'\e[0m'
export LESS_TERMCAP_so=$'\e[01;33m'
export LESS_TERMCAP_ue=$'\e[0m'
export LESS_TERMCAP_us=$'\e[1;4;31m'
```
