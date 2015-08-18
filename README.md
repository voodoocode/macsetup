# My Mac OSX Setup

- Update MacOS X
- [iTerm2](#iterm2)
- [Homebrew](#homebrew)
- [Atom](#atom)
- [Node.js](#node)
- [Oh MY ZSH](#oh-my-zsh)
- [CLI Tools](#cli-tools)
- [Git](#git)
- [Apps](#apps)


## Update
first an update

## iTerm2
http://www.iterm2.com

solarized dark theme

## Homebrew
needs xcode

http://brew.sh

## Atom
https://atom.io

Atom Packages: minimap, open-recent, highlight-selected, open-in-browser

## Node

Node.js and NPM

http://nodejs.org

    $ brew update
    $ brew install node

## oh-my-zsh
https://github.com/robbyrussell/oh-my-zsh

agnoster theme

## CLI-Tools
- [httpie](https://github.com/jkbrzt/httpie)
- [z finder](https://github.com/rupa/z/blob/master/z.sh)

## Git
Aliases:

    la = "!git config -l | grep alias | cut -c 7-"
    pu = pull
    ps = push

    co = checkout
    cob = checkout -b
    com = checkout master
    cos = checkout stage
    s = status
    st = status
    ct = commit
    c = commit -m
    ca = commit --amend

    up = !git fetch origin && git rebase origin/master

    ss = status --short --branch

    br = branch
    ba = branch -ra
    bd = branch -d
    brd = branch -D

    m = merge --no-ff

    ours = checkout --ours
    theirs = checkout --theirs

    aa = !git add -A && git status -s

    lg = log --date=short --color --graph --pretty=format:'%C(yellow)%h%Creset - %C(cyan)%cd -%C(red)%d%Creset %s %Cgre$
    ls = log --pretty=format:'%C(yellow)%h %Cred%d %Creset%s %C(cyan)[%cn]' --decorate
    ll = log --pretty=format:'%C(yellow)%h %Cred%d %Creset%s %C(cyan)[%cn]' --decorate --numstat
    lds = log --pretty=format:'%C(yellow)%h %ad %Cred%d %Creset%s %C(cyan)[%cn]' --decorate --date=short
    ld = log --pretty=format:'%C(yellow)%h %ad %Cred%d %Creset%s %C(cyan)[%cn]' --decorate --date=relative
    fl = log -u
    whatsnew = log --oneline master..

    rank = shortlog -s -n --all

    f = "!git ls-files | grep -i" --color
    gr = grep -Iin --color
    find = log --pretty=format:'%C(yellow)%h %Cred%d %Creset%s %C(cyan)[%cn]' --graph --grep

    dlc = diff --cached HEAD^
    dl = "!git ll -1"

    bmv = branch -m
    done = "!f() { git branch | grep "$1" | cut -c 3- | grep -v done | xargs -I{} git branch -m {} done-{}; }; f"

    shoot = push origin --delete

## Apps
- [1Password](https://agilebits.com/onepassword)
- [Alfred](https://www.alfredapp.com)
- [Paw](https://luckymarmot.com/paw) REST client
- [Sequel Pro](http://www.sequelpro.com) MySQL client
