# Introduction
## Setting up Git on local machine
1. set user email - `git config --global user.email "email-id"` , has to be the same email address using which you set up an account on github
2. set user name - `git config --global user.name "name"`
3. to see what changes are done using the `git config` command - `git config --list`
4. usually git commands are written in a code editor instead of git bash, for smoother dev operations.
5. open integrated terminal in vscode

## Getting started
1. **clone command** - clone repo on local machine (laptop) - `git clone [https-link]`. (remote repo - github).
2. `cd` - change directory to move within folders in the repo
3. to view all files in the folder - `ls`
4. view hidden files - `ls -a` , you will see a .git folder - folder by github
5. **status command** - `git status` , tells you whether its up to date with the branch. if you modify the file then the status shows a long message indicating there is a change in the files and those changes have not been committed. if you add in a new file or folder, then `git status` shows that there is an untracked file(git is not tracking that file as of now). basically, 
    - untracked : new files that git doesnt yet track
    - modified : changed
    - staged : file is ready to be committed
    - unmodified : unchanged
## Making changes to local repo
1. **add command** - adds new or changed files in your working directory to the git staging area - `git add <file-name>`.
2. **commit command** - it is the record of the change `git commit -m "some message"`, the `-m` is used to write a message.
3. to add all the files - `git add .` , all the files that have changes in them get added.
4. after adding and committing these changes through terminal. you need to push the code to github to view the local repo content to remote repo - `git push origin main`. 
5. TLDR, 
    - github desktop : commit -> push to origin
    - git commands : add->commit->push
11. `origin` - basically means that the copy of project on github, the name of that copy is called origin. 
12. `main` - you can create branches on the remote repo, and we are pushing into the `main` branch.

## Creating new repo on local machine

**init command** - used to create a new git repo from the terminal.
- `git init`
- `git remote add origin <link>`
- `git remote -v` : to verify remote
- `git branch` : to check branch
- `git branch -M main` : to rename branch
- `git push origin main`

* for example in the current folder that you are working in, you create a new folder using `cd ..` -> `mkdir localRepo`. Here are the next steps :

    1. After creating the folder `cd localRepo` -> `ls -a` (to check whether this new folder is a git repo or not, as the .git folder will not appear in the hidden files list) -> `git init` -> `ls -a` (now the .git folder has appeared)

    2. create your files, write the code -> `git status` to check the status as untracked -> `git add .` -> `git commit -m "added inital files` -> `git stauts`

    3. now go to github -> create a new repo -> localRepo -> do not initial readme.md

    4. `git remote add origin <link>` - remote is github, get the link from the new repo you just created on github. 

    5. `git branch` : should return master branch at this stage, which used to be the default branch earlier. but now the default branch in github is the `main` branch. so basically we could 2 things : 
        - create a new branch with the name `main`
        - rename master branch as `main` - `git branch -M main`

    6. now the changes should be pushed for the new repo to github - `git push origin main`. 

    7. `-u` flag could be used to set upstream. this basically means that you let github know that you will be working on the main branch itself. this means you do not need to mention `origin main` everytime in the command. simply use the command - `git push` and that would mean the current committed changes have to be pushed to origin main. it is a shortform.

    8. now you could create `README.md` -> `git add .` -> `git commit -m "message"` -> `git push`










