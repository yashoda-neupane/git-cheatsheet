# git-cheatsheet
## How to push the main branch to remote
1. If you want to push the main branch to remote, and if you are pushing for the first time make sure to execute the below commands:

- git init : for initializing a local repository
- git add . :  to add all your files that the local repository has
- git commit -m ‘commit message’ :  to save the changes you made to those files

2. To push the main repo, you first have to add the remote repo to Git by running git remote add <url>

3. To confirm the remote has been added, run git remote -v

4. To finally push the repo, run git push -u origin <branch-name> (“main” is the name of that branch)
