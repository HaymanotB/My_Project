# Git Assignment

This repository contains the steps and files for the Git assignment.
 The assignment involves creating a new Git repository, working with branches,
 and pushing the repository to a remote GitHub repository.

## Steps 1: Create a new directory in home directory and initialize it as a Git repository
  cd ~ 
  mkdir My_project
  cd My_project
  git init
  git config --global init.defaultBranch main
  git branch -m main
## Step 2: Add a README.md file:

  touch README.md
  git add README.md
  git commit -m "Add README.md file"

## Step 3: Create a new branch called dev and switch in to dev branch 
  git branch dev
  git checkout dev

## Step 4: Create a data directory containing the pheno.csv file:

  mkdir data
  touch data/pheno.csv

## Step 5: Create a scripts directory containing the file myfunction.py:

  mkdir scripts
  touch scripts/myfunction.py
  git add scripts/myfunction.py
  git commit -m "Add myfunction.py file to scripts directory"

## Step 6: ignore tracking
  nano .gitignore
  data/

  git add .gitignore
  git commit -m "Ignore data directory"
  
## Step 7: Merge the dev branch with the main branch and delete dev branch:

  git checkout main
  git merge dev
  git branch -d dev

## Step 8: Create a remote GitHub repository and push the local repository to the remote repository:

  Add the remote repository:
  git remote add origin https://github.com/HaymanotB/My_project.git
  

  Push the local repository to the remote repository:
  git push -u origin main
