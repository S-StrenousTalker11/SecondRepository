# Second Repository.
Pushing a locally created repo onto GitHub.

<br>

# GitHub Part 2
This is my second repository. I created this repository locally in my computer and pushed it onto GitHub.

In the process of pushing this local repo, I learnt:

 - git remote add origin <-link-> --> Connecting the local project to the repository on GitHub.
   The steps I followed were:
    1. Create an empty repository with the same name as the local project on GitHub.
    2. Navigate to the local project directory in the terminal.
    3. Run the above command.
    4. Copy the link of the repository on GitHub to the terminal and paste it after origin.
    5. Press Enter to complete the process.

- git remote -v --> Checking the connection to the repository on GitHub.
- git branch --> Gives the current branch name.
- git branch -M <-BranchName-> --> Renaming the branch.
- git push origin main --> Pushing the local repo to the repository on GitHub.
    - Before doing this, all the files in this project must be added and committed.
- git commit -am "message" --> Adding and committing the changes at the same time.
- git log --> Viewing the commit history.
- git push -u origin main --> Making the current branch as the default branch for adding and committing
  changes. By default, the branch is named main. If you want to use a different branch, you can replace main with the name of the branch you want to use. After using this command a single time, whenever we 
  want to push a change , we can simply use git push without the -u/origin main option. Every branch in a repo has its own upstream, ie. its own remote branch. That is what upstream means. Whenever we create
  branch other than main, we have to connect it to its upstream.

<br>

# Branches

Whenever a single project is being handled by multiple developers, it is a good practice to create multiple branches for each developer. This is because each developer can work on a different branch without affecting the work of other developers and affecting the main project as well as to save time. This is called branching.

Necessary commands
 - git branch --> Gives the current branch name.
 - git branch -M <- BranchName-> --> Renaming the branch.
 - git checkout <-BranchName-> --> Switching to a different branch.
 - git checkout -b <-BranchName-> --> Creating a new branch and switching to it at the same time.
 - git branch -d <-BranchName-> --> Deleting a branch.
 - git branch -a --> Viewing all the branches in the project.

# Merging Branches

Whenever the task taken upon by a side branch is completed, it can be merged with the main branch.

This can be achieved by multiple ways:
- git merge <-BranchName-> --> Is a command to merge 2 branches.
- git diff <-BranchName-> --> to compare commits, branches, files & more.
- Using a PR(Pull Request) --> This is a feature of GitHub that allows you to merge the changes from a branch into the main branch . This is a more formal way of merging branches. It is used when you want to  merge the changes from a branch into the main branch after reviewing the changes. Whenever a side branch pulls ahead of the main branch, we get to make a PR. This PR is then reviewed by a team leader(in a company), and is then merged into the main branch if it is considered appropriate and approved.

To pull the change from GitHub into our local project, we can use the pull command.
 - git pull origin main --> Pulling the changes from the main branch in the repository on GitHub into the main branch in the local


# Gitignore

 Gitignore is a file that is used to ignore certain files and directories in a project. This is
 useful when you don't want to track certain files in your project. For example, if you
 have a project that uses a lot of images, you might not want to track all of them in
 your project. You can add the path to the images in the .gitignore file and Git will
 ignore them.


# Git Tagging

 Git tagging is a way to mark a specific point in the commit history. It is used to mark
 a release or a milestone in the project.

# Git Stashing

 Git stashing is a way to save the changes you have made in your working directory so that you
 can come back to them later.

# Fixing Mistakes

 There can be occasions where we add a change to the staging area, and we want to remove it. Similarly,
 there can be occasions where we want to remove a commit from the commit history. This can be achieved
 by using the following commands:
 - git reset HEAD~1 --> This command is used to remove the last commit from the commit history.
 - git reset HEAD~n --> This command is used to remove the last n commits from the commit history.
 - git reset --hard --> This command is used to remove all the changes from the staging area and the working directory.
 - git reset --soft --> This command is used to remove all the changes from the staging area, but the changes are still in the working directory.
 - git reset --mixed --> This command is used to remove all the changes from the staging area, but the changes are still in the working directory.
 - git revert HEAD --> This command is used to remove the last commit from the commit history.
 - git revert HEAD~n --> This command is used to remove the last n commits from the commit history.

 Removing staged changes(git add)
  - git reset <-FileName-> --> This command is used to remove a file from the staging area.
  - git reset . --> This command is used to remove all the files from the staging area.
  
 Removing committed changes using commit hash
  Every commit has a hash that is unique to it. We can also remove committed changes using this unique
  hash

  - git reset <-commit hash-> --> This command is used to remove a commit from the commit history.
  - git reset <- commit hash-> --hard --> This command is used to remove a commit from the commit history and also remove all the changes from th staging area and the working directory.

  We can learn of the commit hash by using the following command: git log.