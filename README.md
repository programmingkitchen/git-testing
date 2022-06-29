# Git Cheats

## Setup a private Repo and clone

**Remote Repo**
```
https://github.com/programmingkitchen/azure.git
```

**Setup Procedure**
```
echo "# azure" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/programmingkitchen/azure.git
git push -u origin main
```

**Get the Status**
```
git status
```

**Clone**
```
git clone https://github.com/udacity/nd9991-c3-Build-CI-CD-Pipelines-Monitoring-and-Logging-v1
```

## Configuration
**On the Local Host**
```
git config --global user.email "programmingkitchen@gmail.com"
git config --global user.name "Programming Kitchen"

```

**Add Remote/origin**
```
git remote add origin https://github.com/rgranier/headlines.git
git remote add origin https://github.com/rgranier/udacityjenkins1.git
```

**HTTPS (password)**
```git remote set-url origin git@github.com:USERNAME/REPOSITORY.git
git remote set-url origin git@github.com:programmingkitchen/alta3-myk8s.git
```
**Do global config**
```
 ~/Dropbox/PYTHON-PROGRAMS/FLASK/headlines (master)
$ git config --global user.email "rgranier@gmail.com"
$ git config --global user.name "Randall Granier"

$ git config --list
```

## Branching 
**Look at the current remote**
```git remote -v

$ git remote -v
origin https://github.com/rgranier/udacityjenkins1.git(fetch)
origin https://github.com/rgranier/udacityjenkins1.git(push)
```

**Examine the branches (local and remote)**
```
git branch
git branch -r
```

**Examine the branches (local and remote)**
```
git branch
git branch -r
```


**Look at local merged and unmerged**
It looks like when there are commited changes in another branch, then it will show up in no-merged.

```
git branch --merged
git branch --no-merged

~/LOCAL-GIT-REPOS/azure/cheats (main)
$ git branch --no-merged
  develop
```


**Create a new branch & checkout at the same time**
```
git checkout -b fix
```

**Switch Branches**
```
git checkout main
git checkout develop
```


**Add everything to the new branch (maybe not necessary)**
```
git add *
```

**Commit to the new branch**
```
git commit -m 'Fix some stuff'
```

**Commit**
```
git commit -m “my comment“
```

**Merge with the local master (optional)**
This would be if we wanted to make changes in a local branch but push to the master
```
git checkout master
git merge fix
```

**Push the branch (the new branch does not need to exist on origin)**
```
git push origin fix
```

**Delete the local fix branch (without local merge) because it was directly merged into the master on Git Hub.**
```
git branch -d fix # Does not delete remote\
git branch -D fix\
```


** Conflicts

https://phoenixnap.com/kb/how-to-resolve-merge-conflicts-in-git






