# ip2020-git-advanced
Template for InfPALS Git Advanced Workshop.

- https://product.hubspot.com/blog/git-and-github-tutorial-for-beginners


**Step 0: Install git & create Github account**
- https://git-scm.com/book/en/v2/Getting-Started-Installing-Git
- https://github.com/

**Step 1.1:Create a local repository**
- in terminal, move to the directory where you want to put the project
- run `git init` command
- add files
  - either write some codes
  - or use touch command to create an empty file
- to associate a local repo with remote Github repo, use `git remote add origin <URL>`
- use `git remote -v` to check the origin
- to change the remote repo, use `git remote set-url origin <URL>`


**Step 1.2: clone a repo from Github**
- use `git clone <url>` command

**Step 2: Check status of git repo**
- use `git status` command to check files' status

**Step 3: Add/commit files**
- use `git add <filename>` to add files to staging environment 
  (file is not yet been added to a commit, but it's about to be)
- use `git commit -m "Your message about the commit"`
- use `git log` to see all the commits

**Step 4.1: Create new branches**
- use `git branch` to list all branches on the machine
- use `git branch <branch_name>` command to create a new branch 
  (branch allows moving back and forth between "states" of a project)
- to switch to a branch, use `git checkout <branch_name>` command
- or use `git checkout -b <my_branch_name>` to create a new brach and checkout to it

**Step 4.2: Merge branches**
- if you want to merge branch A to master, checkout to master first and use `git merge <branch A>`

**Step 5: Create new repository on Github (if you want to work with a team)**
- to add a local repo that was already created, use `git add remote origin <github_URL>` command

**Step6: Push a change to Github**
- use `git push origin <your_branch_name>` to push a branch 
  ('origin' here is just shorthand for the remote repository's URL on Github)
- this allows others to see the changes you made, and if the repo owner approves, this branch will merge with repo's master

**Step 7: Create a pull request (pr)**
- `git pull origin <branch>`
- this alerts a repo's owners that you want to make some changes to their code, 
  allowing them to review the code before putting changes on the master branch

**Step 8: Merge conflicts**
- Sometimes when there are changes in one file that conflicts with a change in another file 
  and git can't figure out which version to use, you'll have to manually fix it


**Step 9: Get new changes from Github**
- now, to update the local master branch for new changes, use `git pull origin master`




- A great resources: https://www.freecodecamp.org/news/git-cheat-sheet-and-best-practices-c6ce5321f52/#:~:text=If%20you've%20copied%20a,URL%20of%20the%20remote%20repo 
