# zsh-aliases-easy-remember

zsh-aliases easy to remember commands for terminals and servers - If you want to help me make bigger the list, you are welcome, just remember that:

1. The commands need to align to an ACTION example is we are going BACK in the folders structure, we find the command:
```
alias back="cd .."
```
// there are expecions called b and cl = back and clean that are to much often used and easy to remember

2. Name them in camelCase first letter in lowercase

Enter into the area of alias (I call them snips = snippets)
```
nano ~/.zshrc
```
Copy paste
```zsh
# exceptions
alias b="cd .."
alias cl="clear"

alias snips="nano ~/.zshrc"
alias snippets="nano ~/.zshrc"
alias resetSnips="source ~/.zshrc"
alias resetTerminal="source ~/.zshrc"
alias home="cd /"
alias enter="cd"
alias back="cd .."
alias enterHosts="sudo nano /etc/hosts"
alias create="touch"
alias createFolder="mkdir"
alias rename="mv"
alias delete="rm"
alias remove="rm"
alias removeDirectory="rmdir"
alias removeFolder="rmdir"
alias copy="cp"
alias move="mv"
alias show="cat"
alias list="ls -al"
alias clean="clear"
alias currentDirectory="pwd"
alias where="pwd"
```

After paste, save the file and exit editor, run this code to reset the terminal
```
source ~/.zshrc
```
if you want the terminal load the alias everytime you enter you must load the alias this way: run this command
```
nano ~/.bash_profile
```
inside paste this command
```
if [[ -n "$SSH_CONNECTION" ]]; then
    source ~/.zshrc
fi
```

## 🤝 Contributing

### Clone the repo

### Submit a pull request
