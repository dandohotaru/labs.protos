# How to view configs [wiki](http://confluence:8090/display/KIKLOS/Git+Setup)
### show all git settings and corresponding locations
```
git config --list --show-origin
```


# How to manage proxy 
### check proxy
```
git config --global --get http.proxy
```
### setup proxy
```
git config --global http.proxy http://proxyvip1:8080
```
### reset proxy
```
git config --global --unset http.proxy
```


# How to initialize repository
```
git init
git add .
git commit -m "stuff"
git remote add origin [url]
git remote -v
git push origin master
```


# How to add configs
### create a project specific config, you have to execute this under the project's directory.
```
git config user.name "John Doe Project"
```
### create a global config for current user profile
```
git config --global user.name "John Doe Global"
```
### create a system config for current machine
```
git config --system user.name "John Doe System"
```
### cache credentials at repo level
```
git config credential.helper wincred
```


# How to manage branches [wiki](https://www.atlassian.com/git/tutorials/using-branches)

### list branches
```
git branch
```
### create branch
```
git branch [name]
```
### checkout branch
```
git checkout [name]
```
### create and check out 
```
git checkout -b [name]
```
### publish branch
```
git push -u origin [name]
```
### delete branch
```
git branch -d [name]
```
### force delete
```
git branch -D [name]
```
### rename branch to [name]
```
git branch -m [name]
```


# How to manage changes [wiki](todo)

### unpushed commits
```
git log origin/master..HEAD
```
### unpushed diffs
```
git diff origin/master..HEAD --stat --cached
```
### simulate push
```
git push --dry-run
```


# How to manage undos [wiki](https://www.atlassian.com/git/tutorials/undoing-changes)

### reset commit (changes show as modified)
```
git reset HEAD~1
```
### nuke commit (changes are well nuked)
```
git reset HEAD~1 --hard 
```
### revert commit
```
git revert --no-commit [hash]..HEAD
git commit
```
### undo files
```
git checkout [hash] [file.path]
```
### temp switch
```
git checkout [hash]
```
### commit reset
```
git reset --hard [hash]
```
### commit stash
```
git stash
git reset --hard [hash]
git stash pop
```

