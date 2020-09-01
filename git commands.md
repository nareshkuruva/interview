## clone project
  ```
   git clone url (clone the project in specific path)
 ```
## branches
```
  >> git checkout -b <name-of-branch>		(create branch)  <br/>
  >> git checkout <name-of-branch>			(switch branch)
```  
  
  
## pull the code from branch
```
  >> git fetch <br/>
  >> git pull
```

## do code and stage changes
```
git add <file-name OR folder-name>   / git add . (all local changes)
```

## commit and push
```
git commit -m "COMMENT TO DESCRIBE THE INTENTION OF THE COMMIT" 
git push <remote> <name-of-branch>  (Push all commits to remote repository)
eg:: git push origin master
```


merge branch with master branch: <br/>
git checkout <name-of-branch> <br/>
git merge master <br/>

-------------------------
## Stash Changes
------------------------
```
git stash save
(or)
git stash
( or with a message)
git stash save "this is a message to display on the list"
```


### To list the stashed modifications
```
git stash list
```

### To show files changed in the last stash
```
git stash show
```

### So, to view the content of the most recent stash, run
```
git stash show -p
```


### To view the content of an arbitrary stash, run something like
```
git stash show -p stash@{0}

git stash apply "stash@{n}"
```

---------------

### git checkout for Remote Branches
```
git checkout --track origin/plcStaging
```
