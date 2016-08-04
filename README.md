# UsefulTips

#### Some tips to make daily tasks easy on linux and git

##### Useful entries in .gitconfig file
Use `git config --global -e` to bring up .gitconfig file if you are not sure where it is placed. On OSX it is in ~/.gitconfig

````
[color]
        ui = auto
[filter "lfs"]
        smudge = git-lfs smudge %f
        required = true
        clean = git-lfs clean %f
[core]
        excludesfile = /Users/908752/.gitignore_global
[difftool "sourcetree"]
        cmd = opendiff \"$LOCAL\" \"$REMOTE\"
        path =
[help]
        autocorrect = 1
[alias]
        ci = commit
        st = status
        co = checkout
        oneline = log --pretty=oneline
        br = branch
        la = log --pretty="format:%ad %h (%an): %s" --date=short
```

#### To Validate YAML Files:
`ruby -e "require 'yaml';puts YAML.load_file('./$1')"`

#### Git Markdown cheatsheet
https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
