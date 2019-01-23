# Git Flow
Simple git command that is so god damn useful


### initializing a Project
using init:  
**`git init`** will initialize a local git repo

using clone with SSH or Http/s:  
**`git clone ssh://git@github.com/[yourUsername]/[yourTargetRepository].git`**    
**`git clone https://github.com/[yourUsername]/[yourTargetRepository].git`**  
* example `https://github.com/a-m-dev/git-flow.git`  


### Snapshotting
**`git status`** will show you all changes that you made with your files  
**`git add [filename.txt]`** will add that file toy staging area   
**`git add -a`** will add all changed files into staging area  
**`git add .`** will do the same as above   
**`git commit`** will open a vim or nano editor for adding message and commiting  
**`git commit -m 'your message'`** will commit with your message in one line command   
**`git rm -r [filename.txt] `** will remove that file or folder from git    
**`git reset`** will unstage all staged files  


### Branching 
**`git branch`** will show all local branches with a state in the begining of a current branch   
**`git branch -a`** will show all local and remote branches   
**`git branch [newBranch]`** will create a new branch with out switching to it    
**`git branch -d [branchName]`** will remove a branch    
**`git push origin --delete [branchName]`** will rmeove a branch on remote repository    
**`git checkout -b [newBranch]`** will create a branch and switch to it    
**`git checkout -b [branchName] origin/[remoteBranchName]`** creates a new branch and clones the remote brnahc into created branch and switches to it    
**`git checkout -`** switches to the previous branch    
**`git checkout -- [fileName.txt]`** discards all changes to file    


### Merging
**`git merge [branchName]`** will merge a branch to the current repo   
**`git merge [sourceBranch] [targetBranch]`** will merge sourceBranch into targetBranch  
**`git stash`** will dump out all changes into stash and cleant the working repository
(this comes handy when you have an unfinished work and and already have a lot of changed files, then you need to work on a hotfix, in this kind of situations you can use git stash command to clear your working tree and then after you done with your bug and commited to the serve, you can use below command to get the previous changes on your repo)   
**`git stash pop`** will bring back the files that you stashed before   
**`git stash clear`** will clear the stashed files   

