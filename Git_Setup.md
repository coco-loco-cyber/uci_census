# Git Setup on Local Machine (Mac Specific)

### Installing Git on a Mac

Install Homebrew: https://brew.sh    
`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`  

Install Git: `brew install git`  
##### This is the method I used for installing Git.

### Check Installation
`git --version`  
`git status` # If not in an initialized Git folder message will state: "not a git repository"

### Configure Global Settings 
#### For Local Settings use --local

`git config --global user.name 'YOUR NAME'`  
`git config --global user.email 'YOUR EMAIL'`  
`git config --global --list` # Check the Global Configuration

### Initialize a Folder for Your Git Project

`git init`  
`git status`  
##### After initializing, the 'git status' command will show the branch name, current status and any untracked files

### Add Files from Folder to Git Repository Staging Area for Committing  

`git add FILE_NAME`  
`git add .gitignore` # Place the names of files you do not want to commit to repo  

### Add a Remote Repository to Commit Files To  

`git remote add origin URL_OF_REPO`  
##### Obtain the URL at GitHub. Remote repo referenced as 'origin'.    
`git remote -v` # View remote repo information

### Commit Files/Changes From Staging Area to Local Repository  

`git commit` or  
`git commit -m "COMMIT COMMENT OF YOUR CHOICE"`

### Push Changes/Commits to a Remote Repository  

`git push -u REMOTE BRANCH` # Remote = origin, Branch = main (or the branch name you are working on)

##### When pushing to a remote repository you will be asked to enter credentials. This is your GitHub login credentials. I created a token for logging in. Utilize the authentication scheme that works best for you.  

##### Reference:  
##### https://docs.gitlab.com/ee/gitlab-basics/start-using-git.html
