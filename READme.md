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
