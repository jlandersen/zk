# zk
CLI for my zettelkasten setup 📚⌨️. Based on 

## Structure
The structure is kept as simple as possible. All markdowns are stored in a single directory and meant to be searched rather than traversed in some hierarchy. All files are named and titled using the scheme `[year][month][day][hour][seconds] [title]`. Example: `20201208080013 AWS Summit 2020.md`. Everything is standard markdown with two conventions:

* Last lines contains tags (`#aws`) - one tag per line
* Links that references other markdowns are considered note links and will be indexed as such


## Requirements
Everything assumes you have `fzf`, `bat` and `tmux`. On MacOS, install with homebrew:
```bash
$ xargs brew install < dependencies

or

$ brew install fzf bat tmux
```

## Setup
Clone the repo and set environment variables (this assumes zsh):
```bash
$ git clone https://github.com/jlandersen/zk.git ~/zk
$ echo 'export PATH=$PATH:$HOME/zk/bin' >> ~/.zshrc

# markdowns are stored in ~/documents/zettles
$ echo 'export ZK_PATH="$HOME/documents/zettles"' >> ~/.zshrc
```

