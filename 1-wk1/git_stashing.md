Advanced Git Commands
Welcome to the exploration of Advanced Git Commands, designed to enhance your workflow and manage your projects more efficiently. In this section, we’ll delve into the concepts of stashing changes and utilizing .gitignore to streamline your development process.

Stashing Changes
When you’re in the middle of work and need to switch branches to work on something else, but you’re not ready to commit the current changes, Git stash is your friend. It temporarily shelves (or stashes) changes so you can work on a different task.

How to Use Git Stash:

Stashing Your Work: To stash changes, simply run:
   git stash
This command takes your modified tracked files and staged changes and saves them for later use, reverting them to their original state.

Listing Stashes: You can have multiple stashes. To see all your stashed changes, use:
   git stash list
Applying a Stash: To apply the most recently stashed changes and keep the stash for potential later use, run:
   git stash apply
If you want to apply a specific stash, use:

   git stash apply stash@{<stash_number>}
To apply the most recent stash and remove it from the stash list, run:

   git stash pop
Removing Stashes: To clear your stashes if you no longer need them, you can run:
   git stash clear
Or to drop a specific stash, use:

   git stash drop stash@{<stash_number>}
Using .gitignore
The .gitignore file is a powerful tool that tells Git which files or directories to ignore in a project. It’s particularly useful for excluding files that don’t need to be part of your repository, such as temporary files, build artifacts, or sensitive information.

How to Use .gitignore:

Creating a .gitignore File:

Create a file named .gitignore in your project’s root directory.
You can specify patterns to ignore. For example:
 # Ignore all txt files
 *.txt

 # But track this one specifically
 !important.txt

 # Ignore all files in the build/ directory
 build/
Files and directories matching these patterns will be ignored by Git.
Common .gitignore Configurations:

Many programming languages and development environments have common files and directories that should be ignored. You can find templates for .gitignore files tailored to various languages and tools on GitHub’s gitignore repository.
Updating .gitignore:

If you add a pattern to .gitignore for files that were already tracked by Git, those files will continue to be tracked. To stop tracking them, you must explicitly remove them from the repository:
 git rm --cached <file>
Commit your changes after updating .gitignore or removing files.