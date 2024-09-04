## Introduction
1. if alot of people are working on product, which is ideally the case. For sepearte work, seperate branches are made.
2. use of branch - multiple people can work on the same code and merge it.

## Commands
1. `git branch` : to see all the branches that are there and also to see which branch you are on. the branch that you are on is usually highlighted with green color.
2. `git branch -M main` : to rename the branch
3. `git checkout <branch-name>` : to navigate, to move from one branch to another
4. `git checkout -b <new-branch-name>` : to create a new branch
5. `git branch -d <branch-name>` : to delete a branch. you would not be able to delete a branch while you are already in it. you need to switch branches and then delete.
6. once you are in a different branch say branch1, now whatever changes you make will only be reflected in that branch and not in the main one.
7. branches in git are stored as a tree.

