# Git commands cheatsheet: the most useful git commands

## 1. How to navigate to your git project Folder
---
Use `cd` to move between folders. E.g.:
```
cd workspace
cd bdl02_dominikreydt_git_cheatsheet
``` 

Move back with `cd ..`

```
~/workspace/bdl02_dominikreydt_git_cheatsheet$ cd ..
~/workspace$ 
```

Use `ls -l` for easier navigation
```
~/workspace$ ls -l
total 8
drwxrwxr-x 3 dci dci 4096 Sep  9 15:57 bdl02_dominikreydt_cv
drwxrwxr-x 3 dci dci 4096 Sep 10 09:45 bdl02_dominikreydt_git_cheatsheet
```

With `mkdir` you will create a new directory
```
~/workspace/ mkdir bdl02_dominikreydt_git_cheatsheet
```

Use `rm` to remove a empty folder and `rm -f` to delete the directory with the files in it.



## 2. Check the status of the project

I can use these commands anytime

- `git status`

>With `git status` I can see if some changes have happened and if some files are ready to be committed.
It gives me an overview of the project at that specific moment in time.


- `git log`


- `git diff`