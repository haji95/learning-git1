
# learning-git1
```
git add .
git rm -r --cached
git commit -m "Messege should be clear and shows what changed"
git commit --amend -m "" to modify a commit
git push
git pull
git branch for local '-r for remote' '-a all branches'
git branch 'name of the branch' to create a new branch
git checkout 'branch name' to switch to a branch
git checkout -  switch to the previous branch
git checkout -b 'branch name' creates a branch and switches to directly
git branch -d 'branch name' to delete a branch 
git oull -r origin main  to rebase

git merge 'branch name' merges the current branch with the named branch by adding the changes to it. NOT RECOMMENDED

git status
git log ir git log --oneline to show each log in one line without much details
ls 
cd
touch 
git show commit number from git log
vi filename to open files then i to insert. When finished press esc then : then wq
cat to output a file
git diff the differnce between working directory and what has been commited
git restore filename to discard changes
```
READ ME FILES ARE IMPORTANT, TAKE CARE OF THEM AND BUILD UP YOUR PROFILE AND MAKE A LITTLE NICE

commits are insinde branches



files --git add--> staging area --git commit--> commit history --git push--> github repo online 


Workflow: 
first thing: if working on a feature pull firstly the changes from master branch from remote to local machine then
a new branch 'git checkout -b branchName'
It adviseble to bring the changes from master into your local machine "rebase". You may have conflicts with main.
To resolve conflicts squash all local commits to one and then stash the commit "a.i. put it aside for the time being"
bring all the changes from main and then try to bring your commit ontop of it. In this way you don't have to deal with 
whole lot of confilcts if you're orginally having several commits.
Then you push to remote, raise a pull request and you have your code checked. If your code is approved, you merge your changes
to the main branch

Rebase: when you checkout a branch and work on it, after a time this branch in remote would be worked on
that means that the status of your branch would be old now. So to bring all the commits that have been done in the main branch
you do a rebase. Basically while rebasing all of your commits gets moved aside then the new commits of the main branch get added, after that 
git try to add your commits to the updated branch. 

https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax