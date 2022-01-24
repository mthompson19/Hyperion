# Using Git and Github on Hyperion
## Check to see if Git is installed on the hyperion (it should be)
### Mine was git version 1.8.3.1

***
## Configure Git
### Add username 
git config --global user.name "Your Username"

### Add email 
git config --global user.email youremail@email.edu

### Check the Configuration 
git config --list
#### It should list your username, email, and init. defalut branch. 

***
## Clone with HTTP 
### Go to the directory you want to clone to Github 
git clone http://github.com/username/repo.git 

### Convert local directory to repository 
git init 

### Add a remote 
git remote add origin youremail@email.edu:username/repo.git
git remote -v 

### Download latest changes 
git pull http://github.com/username/repo.git branch 
#### branch is typically main 

### check status 
git status 

*** 
## Push to Github
#### if necessary move file to the same directory where the README file is now located in your terminal 

### Add file or folder
git add file name or folder 

### Confirm addition 
git status 

### Commit changes 
git commit -m "Comment on change" 

### Push Changes 
git push http://github.com/username/repo.git 

#### it will ask for username and password
#### Since two step verification is required for hyperion use your PAT for your password
#### here is an article on how to get your PAT https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
