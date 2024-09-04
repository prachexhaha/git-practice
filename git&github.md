#Introduction
##key points
1. any change in the file/code has to be first added and then committed. on github add step is skipped. but through git, one needs to add and then commit those changes.
2. to add text to the next line in readme file use - "<br>"
3. commit message does not change the name of the readme.md file. you that as an update message for readme.md file.
4. set user email - `git congif --global user.email [emailid]` , has to be the same email address using which you set up an account on github
5. set user name - `git config --global user.name [name]`
6. to see what changes are done using the `git config` command - `git config --list`
7. usually git commands are written in a code editor instead of git bash, for smoother dev operations.
8. open integrated terminal in vscode

#basic git commands
1. clone command - clone repo on local machine (laptop). remote machine is github - `git clone [https-link]`.
2. `cd` - change directory to move within folders in the repo
3. to view all files in the folder - `ls`
4. view hidden files - `ls -a` , you will see a .git folder - file by github
5. status command - `git status` , tells you whether its up to date with the branch. if you modify the file then the status shows a long message indicating there is a change in the files and those changes have not been committed. if you add in a new file or folder, then `git status` shows that there is an untracked file(git is not tracking that file as of now). basically, 
- untracked : new files that git doesnt yet track
- modified : changed
- staged : file is ready to be committed
- unmodified : unchanged
6. add command - adds new or changed files in your working directory to the git staging area - `git add <file-name>`.
7. commit command - it is the record of the change `git commit -m "some message"`.

