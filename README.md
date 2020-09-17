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

    Messages given by `git status`:
    
    - > working tree clean

    This means that no change has happenend in our project since our last `git commit`

    - > nothing to commit

    This means that no `git add` hass happened yet, so there is no change to commit

    - > changes to be committed

    This means that we have staged some changes with `git add .`, and we now need to commit

    - > changes not staged for commit

    This means that we need to use `git add .` to prepare some changes to be committed



- `git log`

This command shows the commit logs

- `git diff`

Shows what changes have happened in our project since the last `git add .`
- Lines marked in **red** are lines that were removed.
- Lines marked in **green** are lines that were added.
___
---
## 4. Save changes
---

1. `git add .` (or `git add -A`)

    Tells Git that you want to include the latest changes in the next commit. However, changes are not actually recorded until you run `git commit`.
    
2. `git commit -m "meaningful message here"`
    
    A commit is the Git equivalent of a "save". Commits can be thought of as snapshots of our project at a given point in time.

    You can also *quick-commit* by running `git commit -am "explanation and so on"`

    To change a commit use `git rebase -i HEAD~3`
     and follow the introductions in the file.

3. `git push` 
 
   This command sends the committed changes to a server. It is used to upload local repository content to a remote repository.

## 5. Branching

1. `git branch` or `git branch -l` will show your branches

2. `git branch branch-name` create a new branch.
    **Attention** this will not move you to the new branch.

3. `git checkout branch-name` switch to the new branch and work from there

4. Type `git add -A`, `git commit -m "commit over 9000"` and `git push --set-upstream origin branch-name` to update the new branch on github. Now you can `git push`, for shure.

``` From now on you work in the new branch and the Masterfile is saved on the gitHub Server. ```

5. To delete a branch you have to leave the branch into another branch with `git checkout master` (or any other branch). Once that is done it is possible to delete the branch with `git branch -d branch-name` / to force `git branch -D branch-name`.


## Cloning

To clone a repository from github simply use `git clone https://github.com/example_rep/example_rep.git` 

If you want to commit updates to the cloned repository owner, make shure that you have the rights to upload changes from the software owner.
***

`git fetch`

The git fetch command downloads commits, files, and refs from a remote repository into your local repo. Fetching is what you do when you want to see what everybody else has been working on.

***

Assuming:
- we are on a separate branch. Note: it can be checked by running git branch -l
- we have added and committed all our changes
we are now ready to merge our changes back to the main branch (which is usually master). It's time to:

1) Move to branch that you want to merge your changes on.

    E.g: `git checkout master`
    
    After checking out on master, its always good practice to pull the latest changes from the origin with:
    `git pull`
    
2) Merge the changes from the source branch (the one where we committed our changes on) with:
    `git merge my-username/source-branch`
Save our changes to the server.

3) `git push` and you are ready to go.

***

## FYI

| All hail to the CHOSEN ONE the son of the all mighty TERMINAL of all time! Praise the holy KERNEL for his givings in the universe. | lol | OMFG! |
|---|:---:|---:|
| **A table row to crush them all to the deepest ground off evil hell. This column will be filled with the bold text of boldness.** |`A centre aligned tabel column for the holy lord known as THE CHOSEN ONE.` | *Right alignment for right columns. To praise the great eternity of the all mighty TERMINAL!* |





![GitHub Logo](https://github.githubassets.com/images/modules/logos_page/Octocat.png)

# :shit: :skull_and_crossbones: :point_right: :ok_hand: :llama: :fries: :godmode: 1 Number to be removed.


