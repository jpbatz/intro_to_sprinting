Rough gist of thoughts for the git lesson...

#### Note: need to remove the hyperlink (underline)
#### Note: Markdown does not like angle brackets? - affects linefeeds?  

git config --global user.name "Your Name here"  
git config --global user.email "your_email@domainname.com"  

cd to desired dir or folder  

## clones to your local machine  
### creates default remotes to/from origin  

### ssh  
git clone git@github.com:your_username/the_project /local/dev/path  ? if not already in dir
or  
### https
git clone https://github.com/your_username/the_project.git  

### creates remote to original repo
git remote add upstream https://github.com/<main_repo>/the_project.git  

### shows list of remotes
git remote -v

## working with feature branches
? git branch branch_name  

### creates feature branch and switches to it
git checkout -b branch_name  

### shows list of branches and indicates current branch
git branch -v  

### switch to branch
git checkout branch_name  

## when origin/master is ahead of local master, must pull before push
git pull upstream <branch>  

## commits changes  
### with short comment
git commit -m 'hopefully relevant message about this commit'  

### with extended comment (ESC :wq to save and exit)
git commit  

### with extended comments and signature (ESC :wq to save and exit)
git commit -s  

## pushes changes to origin
git push remote_name branch_name  

### or, first time during session to establish default
git push -u remote_name branch_name
### subsequent push uses above 
git push
