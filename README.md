# GIT

## What is GIT?
Git is a distributed version control system (VCS) for tracking changes in computer files. Several commnents on GIT is given as belows:
1. Git enables coordination between multiple developers
2. Git lets us know who made what changes and when
3. Git allows reverting back codes at any time
4. Git allows using both local and remote respositories

Some concepts of Git are:
1. Keep track of code history
2. Takes snapshots of your files
3. You decide when to take a snapshot by making a "commit"
4. You can revisit any snapshot at any time
5. You can stage files at any time
   
## Git's basic commands
1. Downloading the latest version of a remote project and copying it to the selected location on the local machine:
   - `git clone <repository url>` $\rightarrow$ clone whole projects
   - `git clone <repositiry url> -b <branch name>` $\rightarrow$ clone a specific branch
2. Stage changed files (tell Git save these files)
   - `git add <file path>` $\rightarrow$ stage a specific file
   - `git add .` $\rightarrow$ stage all files. Note that we can let git know some files that are not necessary to track by adding their paths into `.gitignore` file
3. See which changes have been staged, which haven’t, and which files aren’t being tracked by Git.
   - `git status`
4. Display the url of the remote repository
   - `git remote -v`
5. Push files to the remote repository
   - `git push origin` $\rightarrow$ by default update all commited files of all branches in the remote repository
   - `git push origin <branch name>` $\rightarrow$ update all commited files of `<branch name>` in the remote repository
6. Get latest updates from the remote repository
   - `git pull`
7. Show all of the tracked files that have been committed:
   - `git ls-tree --full-tree --name-only -r HEAD` $\rightarrow$ on the current branch
   - `git ls-tree --full-tree --name-only -r <branch name>` $\rightarrow$ on the a specific branch


## Some steps to configre using git for the first time at local machines
1. Using `git init` to create a git repository ".git" (git folder)
2. Config user's name and email adress (use `git config --list` to see all configuration):
   1.  `git config --global user.email "thai.nguyenvan9495@gmail.com"`
   2.  `git config --global user.name "Thai Nguyen"`

