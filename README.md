# zsh-aliases-easy-remember

Easy-to-remember Zsh aliases for terminals and servers.  
This project focuses on **action-based aliases** that are readable, intuitive, and consistent.

## Motivation

Short or cryptic aliases are hard to remember, especially when working across multiple servers.  
These aliases are named by **what you want to do**, not by the command itself.

## Quick Start

1. Open your Zsh configuration file:
```sh
nano ~/.zshrc
```

2. Copy and paste the aliases:
```zsh
# exceptions (very common shortcuts)
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

3. Reload the configuration:
```sh
source ~/.zshrc
```

4. (Optional) Load aliases automatically on SSH:
```sh
nano ~/.bash_profile
```

Paste:
```sh
if [[ -n "$SSH_CONNECTION" ]]; then
    source ~/.zshrc
fi
```

## Usage

Aliases are named by **action**, not by command.

Example:
```sh
back
```
Moves one directory up (`cd ..`).

### Rules
- Use **camelCase** (first letter lowercase)
- Alias names must describe an **action**
- Only two exceptions: `b` (back) and `cl` (clear)

## Contributing

Contributions are welcome 🤝

### Clone the repo
```sh
git clone https://github.com/sixteen-core/zsh-aliases-easy-remember.git
```

### Submit a pull request
- Add action-based aliases
- Follow naming rules
- Keep it simple and readable
