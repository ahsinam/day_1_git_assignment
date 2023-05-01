1. Can we have global .gitignore?
   Along with the repository specific .gitignore, we can even have a global .gitignore. 
   Inorder to create a global .gitignore, we ought to be in the home directory in the terminal. Next, we use the touch command to create the .gitignore_global file.
   Then, just as in a typical .gitignore file, open the file in preferred text editor and add the patterns for the files or directories one wish to ignore and save the file. Lastly, run the command git config --global core.excludesfile ~/.gitignore_global to instruct git to utilize the global.gitignore file.

2. How do you find difference between two commits?
   "git diff" is used to check the difference between two commits which calls the "diffing function". This function takes two parameter as input which are essentially the commits of the file, and marks difference between those parameter. 

3. Write a difference between git add and git commit command.
   While the git commit command permanently writes changes to the repository, git add simply adds changes to the staging area.

4. How to unstage files?
   We use git restore --staged [filename] command to unstage the files.

5. How to revert a commit ?
   In order to revert a commit we use the command git revert [id_of_commit].

6. Difference between revert and reset? 
   In case of revert, a prior commits modifications are reverted in a fresh commit whereas, in case of rest, it modifies the staging area. 

Day 2

2.a. Write the difference between fetch and pull command.
   Pull Command fetch and download the content from the remote repository and immediately update the local repository whereas on the other hand pull just fetch the content from the remote repository without merging the content.

2.b. How to handle merge conflicts?
   The steps to handle the merge conflicts are:
   1. Pull the latest changes
   2. Idenfity the conflicts
   3. Understand the changes
   4. Resolve the conflicts
   5. Test and Commit the changes
   