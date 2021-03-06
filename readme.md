Collection of most frequently used git commands
======
Git basics - Pushing files to Remote
```javascript
git add .
git  commit -m 'Message'
git push origin master
```

Git reset local changes
```javascript
git reset --hard HEAD
git clean -f -x -d -n
```

Git reset local changes before push
```javascript
git reset --hard HEAD~1
```

Check existing remote URL
```javascript
git remote -v
```


Git add remote URL
```javascript
git remote add origin git@github.com:username/repo.git
```

Git change remote URL
```javascript
git remote set-url origin git@github.com:username/repo.git
```

Reset git add. before commit
```javascript
git reset
```

Sync a fork
Add Upstream
```javascript
git remote add upstream git@github.com:username/repo.git // main form url
git fetch upstream  // fetch upstream to local
git merge upstream/master  //merge to master
git push origin master
```

See changes in file
```javascript
git diff filename
```

Get latest commit hash
```javascript
git rev-parse HEAD -- full hash
git rev-parse --short HEAD --> short hash
```

Back to previous branch 
```javascript
git checkout -
```

Create new branch in Local and push to origin
```javascript
git checkout -b branch-name
git push origin branch-name
```

Revert Merge
```javascript
git merge --abort
```

Rebasing
```javascript
git rebase master
git push -f origin branch-name // -f is important here
```

Revert pushed rebase
```javascript
 git reflog
 git reset --hard HEAD@{10}
 git push -f origin branch-name
 ```

Delete local branch
```javascript
git branch -d branch_name
git branch -D branch_name // force delete
```

