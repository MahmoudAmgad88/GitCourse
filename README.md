# GitCourse with Ossama Elzero
For ElZero Course Git Course
## Basic writing and formatting syntax link
* https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
## 03 create github repo and clone it to you local disk
* download cmder
* cd cmder_mini
* mkdir My-Github
* Copy HTTPS code from your repo
* from cmder type <git clone "then past your copy">
* ls
* cd My-Github
* dir
## 04 Add rest commit
* Use `git status` to show you what branch you're on, what files are in the working or staging directory, and list all new or modified files that haven't yet been committed.
* Use `git add *` or `git add [filename]` like `git add css\main.css index.html`to adds new or changed files in your working directory to the Git staging area.
* Use `git reset [filename]` or `git reset head salakawy.rtf`if you neee to perform unstaging.
* you may have to excute below two commands at firts time for authentication:
 ```
  git config --global user.email "eng.salakawy@gmail.com"
  git config --global user.name "MahmoudAmgad88"
```
* Use `git commit -m "descriptive message"`: Records file snapshots permanently in version history from staging to local repo

### 04 all needed Git commands are:
```
git status
git add [filename]
git reset [filename]
git commit -m "descriptive message"
```


