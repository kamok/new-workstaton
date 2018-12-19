# new-workstation
Things to install when at a new workstation

### Basic Apps
1. Chrome
1. iTerm2
1. LastPass
1. Slack
1. Spotify
1. G-Suites
1. Alfred
1. VSCode - use Cmd + P and "> path" to get it on path too!

### Bash Profile
```
# Git Aware Prompt - https://github.com/jimeh/git-aware-prompt
export GITAWAREPROMPT=~/.bash/git-aware-prompt
source "${GITAWAREPROMPT}/main.sh"

# PS1
export PS1="\[$txtblu\]\w \[$txtgrn\]\$git_branch\[$txtred\]\$git_dirty\[$txtrst\]\$ "

# Aliases
alias bp='code ~/.bash_profile'
alias load_bp='source ~/.bash_profile'
alias be='bundle exec '
alias reset1='git reset --soft HEAD~1'
alias up='!git fetch origin && git rebase --autostash'

# mkdir + cd
mkdircd() {
	mkdir -p -- "$1" && cd -P -- "$1"
}
```

### Colors
iTerm2 https://github.com/YabataDesign/afterglow-itermcolors
Git https://github.com/jimeh/git-aware-prompt

### GitX
https://github.com/rowanj/gitx

### Homebrew
https://brew.sh/

### Rbenv
https://github.com/rbenv/rbenv
