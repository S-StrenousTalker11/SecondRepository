# Second Repository.

Pushing a locally created repo onto GitHub.

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