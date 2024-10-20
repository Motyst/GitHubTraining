# Git and GitHub Beginner Tutorial

## Table of content 

### 1. Installing Git

1. Install Git on your system
2. Create a local repository

### 2. Connecting your Git with your GitHub account

1. Create a SSH key on your computer
2. Register a GitHub account
3. Connect your Github account with your public key
3. Make your first GitHub repository
4. Connect local repository with GitHub repository

### 3. Git commands and usage

1. Add, commit and push your first update
2. Git Hash, Log and Head
3. Amend last commit
4. Restore and reset commands
5. View changes in files
6. Ignoring file

### 4. Working with Github repositories

1. Cloning other repositories
2. Forking project
3. Creating and managing branches

---

## 3. Git commands and usage

### 3. Amend last commit

**Main concepts:**

* ```--amend``` works only with the last (HEAD) commit.
* To add new files to the last commit use command ```git commit --amend --no-edit.``` (Message will remain the same)
* To change message of the last commmit use command ```git commit --amend -m "New commit message"```


### 4. Restore and reset commands

**Main commands:**

* ```git restore --staged <file>``` moves file from *staged* to *modified* or *untracked*
* ```git reset --hard <hash>``` resets the history to the *commit* with hash 
* ```git restore <file>``` resets changes that are not yet *staged* nor *commited*

### 5. View changes in files

**Main commands:**

* ```git diff ``` view changes in *modified* files
* ```git diff --staged``` view changes in the *staged* files  
* Command ```git diff <commit1> <commit2>``` shows all changes that happened between commit1 and commit2

### 6. Ignoring files

**Main ieas:**

* File ```.gitignore ``` allows to add list of files that should be ignored by git
* What files are being ignored can be seen using command ```git status --ignored```
* Examples of how to mark text (*text file used as example*) files to be ignore includes ```.txt``` -- ```/.txt``` -- ```**.txt``` -- ```main/*/.txt```

---

## 4. Working with Github repositories

### 1. Cloning other repositories

**Steps for cloning:**

1. To clone repository from Github press "code" and select it's ssh link. 
2. Use command ``` Git clone <link> ``` to clone repository

### 2. Forking projects

Forking allows to copy someone elses github repositoty into your own Github account and then adding whatever changes you want. 
That's done usually when you don't have access to change the original repository.

### 3. Creating and managing branches

**Branches - How To:**

1. To create a branch use command ```git branch <name>```
2. To view branch use command ```git checkout <branch-name>``` & use ```git checkout -b <branch-name>``` to create a branch and switch to it.
3. View existing local branches using ```git branch``` & remote repository branches using ```git branch -a```