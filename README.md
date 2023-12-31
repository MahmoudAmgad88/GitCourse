# GitCourse with Ossama Elzero
For ElZero Course Git Course
## Basic writing and formatting syntax link
* https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
## 03 create github repo and clone it to you local disk
* download cmder
* download github
* open cmder then creat folder `mkdir My-Github`
* ceate new repo in github with `README file` then Copy HTTPS code from your repo
* from cmder type `git clone [HTTPS code link from your repo]`
* excute below commands to confirm your downloads:
```
ls
cd My-Github
dir
```
## 04 Add rest commit
* Use `git status` to show you what branch you're on, what files are in the working or staging directory, and list all new or modified files that haven't yet been committed.
* Use `git add *` or `git add [filename]` like `git add css\main.css index.html`to adds new or changed files in your working directory to the Git staging area.
* Use `git reset [filename]` or `git reset head salakawy.rtf`if you neee to perform unstaging.
* you may have to excute below two commands at firts time for authentication:
 ```
  git config --global user.email "eng.salakawy@gmail.com"
  git config --global user.name "MahmoudAmgad88"
```
* Use `git commit -m "descriptive message"`: Records file snapshots permanently in version history from staging area to local repo

### 04 all needed Git commands are:
```
git status
git add [filename]
git reset [filename]
git commit -m "descriptive message"
```

![Scr](https://github.com/MahmoudAmgad88/GitCourse/assets/54455617/ccdf5282-c724-4817-880f-1617489429d8)

## 05 Push Local Changes to Remote repo
* Use `git branch` to know all your branshes in local repo
* Use `git remote -v` to know your remote repo.
* Use `git push RemoteName BranshName` to uploads all local branch commits to the corresponding remote branch.
* hint: Updates were rejected because the remote contains work that you do not have locally
       - This is usually caused by another repository pushing to the same ref.
       - You may want to first integrate the remote changes(e.g., 'git pull ...') before pushing again.
  
## 06 Git Pull
* Use `git pull RemoteName` to fetch and download content from a remote repository and immediately update the local repository to match that content

## 07 every thing about git configuration
*  `git config --list`
*  `git help config`
*  `git config --global user.email`
*  `git config --global user.name`
*  `git config --list --show-origin`
*  `git config --global --unset user.name`
*  `git config --global user.name MahmoudAmgad88`
*  `git config --global --edit`

## 08 Generate and test github public kay
* Use `ssh-keygen -t rsa -b4096 -C "eng.salakawy@gmail.com"` to generate ssh keygen
* Use `cat ~/.ssh/id_rsa.pub` to read your ssh keygen
* from your github web got to setting in your profile then select setting then choose SSH and GPG keys then choose add key
* Use `ssh -T git@github.com` to test you key working normally.

## 09 Create repo from existing project
* `mkdir repos`
* `cd repos\`
* Use `ssh -T git@github.com` to connected as ssh
* Use `git init` to Initialized empty Git repository in D:/cmder_mini/My-Github/repos/.git/
* Use `touch index.html` to create file
  ```
  git status
  git add index.html
  git status
  git commit -m "trail repos"
  git status
  ```
* go to your github and create new repo
* run command `git remote add origin git@github.com:MahmoudAmgad88/Course2023.git`
* run command `git branch -M main`
* run command `git push -u origin main` this will pulll then push to avoid others modifications

## 10 Learn Pull Request With Real Examples
*  
