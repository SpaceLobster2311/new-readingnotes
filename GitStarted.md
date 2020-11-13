# Getting Started with Git

## Cool Commands for Command line and Terminal

1. ls = List, shows you all files in current directory
2. cd = Choose Directory, allows you to move into new directory. ex cd onedrive
3. cd ~ will bring you to your root  directory
4. clear = will clear console if its too cluttered
5. mkdir = make directory
ex. mkdir demo
6. rm + name of folder will remove file
7. rm -r = remove a directory (recursively)
ex. rm demo
8.  pwd = present working directory.  Will tell you exactly where you are at
9. cd .. = will take you back
9. cp = copy.  Can copy files
10. touch = create file within directory
11. .. = goes back one level, ../ bring you up a level then back down to a different level u choose.

**A / is seperating directories**

  11.a ../.. moves up 2 levels
12. touch ../ = means create a file one level above me
13. mv = move file. ex mv (file name)


###### Prerequisites
It is highly recommended you have a solid understanding of Terminal or Command Line

## Version Control
Version control is a system that allows you to revisit various versions of a file by recording changes. Git is a DCVS or **Distributed Version Control Systems** which 
allows collaboraters to work together even if one centralized version control goes down. 

## So what is Git

Allows us to track all changes across team. It's the same file with a history behind it. 

##### Snapshots
Commits represent each successive version of a file or files
Each successive snapshot in time
Commit message is just a description of what changed
  * you can assign messages to commits.
Your HEAD = the label meaning "you are here"
Use Git to take snapshots of your code at points in time
Git keeps a histroy of what those snapshots look like.
Usually you give a snapshot label a message. 

## What is GitHub?
* A way to share code with others!
* An online place to store your code (Backup is good)
* It uses Git to help manage your teams work:
  * Version Tracking
  * Reviewing Changes
  * Keeping changes seperate until you want to add them

Git + Github = Awesome

* Git is our version control
* Github is the online code storage
* Work on code on your own computer

### Repositories 
AKA repos AKA folders

#####What is a repository?
* A collection of files you told Git to pay attention to
  * Usually its 1 project 1 repository. 
* Repositories can live on teh computer or Github

## Once you create a repository...
You can link it from cloud to computer.

by cloning it.

To do that, you go to the github repository and hit green button that says **Code**

It'll show you a url which u can copy.  

Go into Terminal, create a new project directory, and type git clone,   then paste. 

It'll bring down code from github and bring it to the machine.  

*you only need to clone once*

git remote -v will show you where you got file from.

### ACP workflow
* Add
* Commit 
* Push

After edidting file **git status**

**git add (name of file)** *will turn red to green.*

After adding, you need to commmit file. 

**git commit -m** "initial html file skeleton"

Push. The command is below

**git push origin main**

*asks for username and password*

Pushing will send all item from main branch on pc to main on github. 

### Class Cheat Sheet

cd = Change Directory

ls = List all the files in the directory

pwd = Present working directory, where you are currently at

cp {where the file is located} {where you are moving it to} = copy/clone a file to a new location

mv {where the file is located} {where you are moving it to} = move the file to a new location

rm = remove a file

rm -r = remove a directory (recursively)

mkdir = create a new directory

touch = create a new file (don't forget the extension!)

git clone {url} = clone a repo from GitHub to your local machine

git status = check if there are any red/untracked changes to your repository (green means it's being tracked!)

git add . = add all the files that need to be tracked 

git commit -m "enter message here" = add a caption/message to your commit/snapshot

git push origin main = send the code up from your local machine to the cloud/GitHub
   
  
### Command line demo results:
* zom8@DESKTOP-AKPS6QD:/mnt/c/users/alexw$ mkdir Alexander
* zom8@DESKTOP-AKPS6QD:/mnt/c/users/alexw$ cd Alexander
* zom8@DESKTOP-AKPS6QD:/mnt/c/users/alexw/Alexander$ touch index.html
* zom8@DESKTOP-AKPS6QD:/mnt/c/users/alexw/Alexander$ pwd
/mnt/c/users/alexw/Alexander
* zom8@DESKTOP-AKPS6QD:/mnt/c/users/alexw/Alexander$ mkdir test
* zom8@DESKTOP-AKPS6QD:/mnt/c/users/alexw/Alexander$ cp index.html test
* zom8@DESKTOP-AKPS6QD:/mnt/c/users/alexw/Alexander$ pwd
/mnt/c/users/alexw/Alexander
* zom8@DESKTOP-AKPS6QD:/mnt/c/users/alexw/Alexander$ touch demo.txt
* zom8@DESKTOP-AKPS6QD:/mnt/c/users/alexw/Alexander$ rm index.html
* zom8@DESKTOP-AKPS6QD:/mnt/c/users/alexw/Alexander$ mv demo.txt test
* zom8@DESKTOP-AKPS6QD:/mnt/c/users/alexw/Alexander$ rm test
* rm: cannot remove 'test': Is a directory
* zom8@DESKTOP-AKPS6QD:/mnt/c/users/alexw/Alexander$ rm -r test
