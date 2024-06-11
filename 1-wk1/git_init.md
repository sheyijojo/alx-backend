## git init

Objective: Learn how to create a file locally, initialize a Git repository, commit your changes, and push the repository to GitHub.

Skills Practiced:

Initializing a Git repository
Basic Git commands (add, commit, push)
Creating a new repository on GitHub
Pushing a local repository to GitHub
Task Steps:

Create a New File Locally:

On your computer, create a new directory named LocalRepoProject.
Inside this directory, create a file named hello.txt.
Open hello.txt in a text editor and add the following content:
 Hello, Git and GitHub!
Initialize a Git Repository:

Open a terminal or command prompt.
Navigate to the LocalRepoProject directory.
Run the following command to initialize a new Git repository:
 git init
Commit Your File to the Repository:

Add hello.txt to the staging area with the command:
 git add hello.txt
Commit the file to your repository: git commit -m "Add hello.txt with greeting"
NB: By default Git will create the a master branch but it is now recommended to have your default branch as main instead. Hence run the command below to set your default branch to main

git branch -M main
Create a New Repository on GitHub:

Log in to your GitHub account.
Click the New button (or navigate to this link) to create a new repository.
Name your repository LocalRepoProject. Do not initialize the repository with a README, .gitignore, or license.
Click Create repository.
Push the Local Repository to GitHub:

After creating the repository on GitHub, you’ll be shown a URL for the repository. Copy this URL.
Back in your terminal, link your local repository to GitHub with the command:
 git remote add origin <REPOSITORY-URL>
Push your commits to GitHub:

 git push -u origin main
Expected Outcome:

You will have a local Git repository with a single file (hello.txt) committed. This repository will be pushed to GitHub, where the file will be visible in your new LocalRepoProject repository.

Submission:

We have access to your GitHub account so the checker will be able to directly check your submissions. Ensure your repository is public so it can be reviewed by the checker.

Notes:

This project is designed to introduce the fundamental workflow of using Git locally and pushing changes to a remote repository on GitHub.
Ensure you replace <REPOSITORY-URL> with the actual URL provided by GitHub when you create your online repository.
Repo:

GitHub repository: LocalRepoProject
File: hello.txt