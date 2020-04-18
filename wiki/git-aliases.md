# Git aliases

## Aliases in CMDER

add the following lines to `%cmder_root%\config\user_aliases.cmd`

```cmd
ls=ls --show-control-chars -F --color $*
gpub=git push --set-upstream origin $*
gl=git log --oneline --all --graph --decorate  $*
gum='git checkout master && git fetch origin && git reset --hard origin/master $*'
gst=git status -sb
grm=git pull --rebase origin master
```
