# Commands


_A list of my commonly used commands_

--

### OS Commands

| Command | Description |
| ------- | ----------- |
| `pwd` | Know the current directory you are in. |
| `cd or cd ~` | Navigate to your home directory |
| `cd D:` | Navigate to D directory |
| `cd folder_name/folder_name/` | Navigate to specific folder |
| `cd ..` | Navigate to previous folder |
| `cd ../..` | Navigate to two previous folder |

## Git Commands 


#### Basic Commands

| Command  | Description |
| -------- | ----------- |
| `clear` | Clear bash screen |
| `Ctrl + l` | Clear screen |
| `ls` | Display only non-hidden folders |
| `ls -a`| Display number of available folders in your current folder along with the hidden fields |
| `ls -al` | Display in sequential manner |
  

#### Creating and Cloning project

| Command  | Description |
| -------- | ----------- |
| `git init` | Initialize a local Git repository |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Create a local copy of a remote repository |
| `git clone https://github.com/[username]/[repository-name].git` | Create a local copy of a remote repository |
| `clear` | Clear bash screen |

#### Basic Snapshot

| Command  | Description |
| -------- | ----------- |
| `git status` | Check status |
| `git add [file-name.txt]` | Add a file to the staging area |
| `git add *.extension` | Add all files ending with specific extension|
| `git add -A` | Add all new and changed files to the staging area |
| `git add * (or) git add .` | Add all the folders and files in the folder at once |
| `git rm -r [file-name.txt]` | Remove a file (or folder) |
| `git commit -m "[commit message]"` | Commit changes |
| `git commit -am "[Specify the message]"` | Express Commit|

#### Branching & Merging

| Command | Description |
| ------- | ----------- |
| `git branch` | List branches (the asterisk denotes the current branch) |
| `git branch -a` | List all branches (local and remote) |
| `git branch [branch name]` | Create a new branch |
| `git branch -d [branch name]` | Delete a branch |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git checkout -b [branch name]` | Create a new branch and switch to it |
| `git checkout -b [branch name] origin/[branch name]` | Clone a remote branch and switch to it |
| `git branch -m [old branch name] [new branch name]` | Rename a local branch |
| `git checkout [branch name]` | Switch to a branch |
| `git checkout -` | Switch to the branch last checked out |
| `git checkout -- [file-name.txt]` | Discard changes to a file |
| `git merge [branch name]` | Merge a branch into the active branch |
| `git merge [source branch] [target branch]` | Merge a branch into a target branch |
| `git stash` | Stash changes in a dirty working directory |
| `git stash clear` | Remove all stashed entries |

#### Sharing & Updating Projects

| Command | Description |
| ------- | ----------- |
| `git remote add origin https://github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote -v` | Check whether our repository has been added to remote server |
| `git push origin [branch name]` | Push a branch to your remote repository |
| `git push -u origin [branch name]` | Push changes to remote repository (and remember the branch) |
| `git push` | Push changes to remote repository (remembered branch) |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git pull` | Update local repository to the newest commit |
| `git pull origin [branch name]` | Pull changes from remote repository |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH |

#### Inspection & Comparison

| Command | Description |
| ------- | ----------- |
| `git log` | View changes |
| `git log --summary` | View changes (detailed) |
| `git log --oneline` | View changes (briefly) |
| `git diff [source branch] [target branch]` | Preview changes before merging |
  