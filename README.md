# CoffeeWithCoddingTest
This is a pratice repository for Git & Github Series with inclided all commands.
<br>
Prepared by Shivanand Hatte.
<br>
Setting up Git
<br>
Download   
<br>
           1. Visual Studio Code
<br>           
           2. Windows (Git Bash) --https://git-scm.com/download/win 
<br>           
           3. Mac (Terminal)
 <br>           
To check Vesion of Git...

git --version
<br>
--------------------------------------------------------------------------------
Git configuration

git config --global user.name "shivanand Hatte"
git config --global user.email "shivanandhatte@outlook.com"
To check git congigration setup=>git config --list
--------------------------------------------------------------------------------
Clone and Status

Clone: Clone a repository pn your local machine (code copy from github)
Command: 
git clone <Link>

Status: Display or check status of code.
git status


some additional command for you
cd folder name          --------------go to current working directory
cd mkdir folder name    --------------create new foldergit
cd ..                   --------------go back from working directory
ls                      --------------List the files or folders on working directory
ls -a                   --------------Display hiddne files and folders on working directory
ls -l                   --------------Dispay details of files and folders on wroking directoirt

---------------------------------------------------------------------------------------------------
File ststus

untracted               ------------New file that git dosen't yet track.
mdified                 ------------exisitng file has modified.
staged                  ------------file is ready to committed.
unchanged               ------------fine is upto date.there is no change.

------------------------------------------------------------------------------------------------------
Add abd Commit

add: adds new or changed file in your working derictory to the git satging area.
Command:
git add <-file name->

for add All file
command:
git add .

commit: it is the record to change
Command
git commit -m "some message"
---------------------------------------------------------------------------
Push Command
push: upload local machine repo content to remote repo (github)
command:
git push origin main

origin: it is a default origin 
main: it is defailt main branch


--------------------------------------------------------------------------------
init command

git init        
The git init command is used to initialize a new Git repository in a directory. When you run this command, Git creates a new repository with all the necessary data structures and files required for version control. Here's how you can use it:

git remote add origin <-Link->
Eg: git remote add origin https://github.com/yourusername/your-repo.git

The git remote add origin command is used to set up a connection between your local Git repository and a remote repository. The word "origin" is a commonly used default name for the remote repository, but you can choose a different name if you prefer.

git remote -v
The git remote -v command is used to view a list of remote repositories that are associated with your local Git repository, along with their corresponding URLs. This is useful for checking which remote repositories are configured and verifying the URLs associated with them. Here's how you can use it:

origin  https://github.com/yourusername/your-repo.git (fetch)
origin  https://github.com/yourusername/your-repo.git (push)


git branch
The git branch command is used to list, create, or delete branches in a Git repository. When you run git branch without any arguments, it will simply list all the branches in your repository and indicate the currently checked out branch with an asterisk (*) next to it. Here's how you can use the git branch command

output:
* main
  feature-branch
  another-feature
  In this example, the main branch is currently checked out, as indicated by the asterisk (*).

  To create a new branch
  git branch my-feature


to rename branch
git branch -M main

To switch to a different branch,
git checkout my-feature


Alternatively, you can create and switch to a new branch in a single command by using the -b option with git checkout:
git checkout -b my-feature


To delete a branch, use the -d option followed by the branch name. For example, to delete the "my-feature" branch, run:
git branch -d my-feature
Note that Git will prevent you from deleting a branch that contains changes that haven't been merged. If you want to forcefully delete a branch, you can use the -D option instead of -d.
git branch -D my-feature
The git branch command is essential for managing branches in Git, which is crucial for organizing and developing different features or versions of your code.

git push -u origin main            -------------   -u is use for origin main not type in every push command. 
