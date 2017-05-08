Rough gist of thoughts for the git lesson...

git config --global user.name "Your Name here"  
git config --global user.email "your_email@domainname.com"  

## clone to your local machine
git clone git@github.com:your_username/the_project /local/dev/path  
or  
git clone https://github.com/your_username/the_project.git  

git remote add upstream https://github.com/<main_repo>/the_project.git  
git remote -v

? git branch branch_name  
git checkout -b branch_name  
git branch -v  
git checkout branch_name  
git pull upstream <branch>  
git commit -m 'hopefully relevant message about this commit'

git push remote_name branch_name
