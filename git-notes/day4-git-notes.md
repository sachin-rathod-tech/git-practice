========================================
# Day 4 - Git Branch & Merge Test
========================================

## 1. Install Git
--------------
### Ubuntu:

```bash
sudo apt update -y
sudo apt install git-all -y
```

### Amazon Linux:
```bash
sudo yum install git -y
```

### Check Version:
git --version


# 2. Branch and Merge Setup
-------------------------
```bash
apt update -y
apt install git-all -y
mkdir cloud
cd cloud
git init
```

## Create SSH Key:
### ssh-keygen (All steps on back page)

### Git Clone:
 * git clone (sshlink)

cd directory

### User Config:
```bash
git config --global user.name "sachin"
git config --global user.email "email@example.com"
```

### Check User Config:

* git config --list

## Remote Repo Link to Local Repo Check:
```bash
git remote
git remote -v
```

# 3. Branch Commands
------------------
### Show branch all:
```bash
git branch
```
---
###Create branch:
```bash
git branch dev
```
---

## Switch branch:
``` bash 
git checkout dev (dev is branch name)
switch dev
```
---

## Switch & Create branch:
* git checkout -b branchname
### * test

*  git branch
---

## Branch delete:

* git branch -d name
* git branch  (check branch)
---

## Create file & add data:
```bash
echo "hello mark" > mark.txt
git add mark.txt
git commit -m "mark add"
```
---

# 4. Main Merge & Remote Push
---------------------------
### Go to main branch & merge:
```bash
 git checkout main
 git branch
```
---

### Merge:
* git merge dev (branch-name)

### Push file in main Remote Repository:
```bash
git push
```
---
## Merge -> two branches into one
## Git merge is used to combine change form one branch into another branch
---

### 2nd Way Test:
```bash
git branch
git checkout -b kali
add file
git add .
git commit -m "Hi"
```
* git checkout dev    / You not merge / direct Push
* git merge kali
* git push origin kali
### kali branch all file save in dev branch
---
# Sachin Rathod Notes 
---
