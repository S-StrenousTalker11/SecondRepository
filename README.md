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
  want to push a change , we can simply use git push without the -u/origin main option.

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