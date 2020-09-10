# Git commands cheatsheet: the most useful git commands


## 1. How to navigate with the Ubuntu terminal to your git repository folder
---
Use `cd` to move between folders. E.g.:
```
cd workspace
cd bdl02_exampleguy_git_cheatsheet
``` 

Move back with `cd ..`

```
~/workspace/bdl02_exampleguy_git_cheatsheet$ cd ..
~/workspace$ 
```

Use `ls -l` for easier navigation
```
~/workspace$ ls -l
total 8
drwxrwxr-x 3 dci dci 4096 Sep  9 15:57 bdl02_exampleguy_cv
drwxrwxr-x 3 dci dci 4096 Sep 10 09:45 bdl02_exampleguy_git_cheatsheet
```

With `mkdir` you will create a new directory
```
~/workspace/ mkdir bdl02_exampleguy_git_cheatsheet
```

Use `rm` to remove a empty folder/file and `rm -f` (force) to delete the directory with the files in it.
```
~/workspace/ rm bdl02_exampleguy_git_cheatsheet
```
Make a file withe `touch`
```
~/workspace/bdl02_exampleguy_git_cheatsheet/ touch README.md
```

Rename a file with `mv`
```
~/workspace/ mv REDME.md README.md
```

___

---
## 2. Initialize a new git repository
---

If any `git` command that we run gives the following output:

>fatal: not a git repository (or any of the parent directories): .git

it means that we are not inside a git repository.

In such case we can:

1. Make sure that we are in the right folder
2. Initialize git repository

To initialize a new repository simply use `git init`
```|
~/workspace/bdl02_exampleguy_git_cheatsheet/ git init
```
Once this is done your new git repository is ready to go.
___
---
## 3. Check the status of the repository
---
I can use these commands anytime, while you editing your files

- `git status`

    With `git status` I can see if some changes have happened and if some files are ready to be committed.
    It gives me an overview of the repository at that specific moment in time.


- `git log`


- `git diff`

___
---
## 4. Save changes
---

1. `git add .` (or `git add -A`)

    Tells Git that you want to include the latest changes in the next commit. However, changes are not actually recorded until you run `git commit`.
    
2. `git commit -m "meaningful message here"`
    
    A commit is the Git equivalent of a "save".

3. `git push` 
 
    This command sends the committed changes to a server. It is used to upload local repository content to a remote repository.






