# git-cheatsheet
## How to push the main branch to remote
1. If you want to push the main branch to remote, and if you are pushing for the first time, make sure to execute the below commands:
   *** git init: for initializing a local repository
   ***  git add . :  to add all your files that the local repository has
   *** git commit -m ‘commit message’ :  to save the changes you made to those files

3. To push the main repo, you first have to add the remote repo to Git by running git command as - 
     - git remote add origin <git URL for the repo>
     eg : git remote add origin https://github.com/yashoda-neupane/java-8-features-review.git


4. To confirm the remote has been added, run
    - git remote -v

5. Before pushing the code need to pul the code from the remote, use below command
    - git pull origin main --rebase  # Reapplies your commits on top of remote changes
    - What happens?

        - Your local commits are rewritten to appear after the remote changes.

        - Results in a cleaner, linear history (preferred for shared branches).
    If conflicts occur:

          1. Resolve them in IntelliJ (Git tool window).

          2. Continue rebasing:
             - git rebase --continue
          3. git rebase --continue
              -  git push origin main


7. To finally push the repo, run
   - git push -u origin <branch-name> (“main” is the name of that branch)
   eg : git push -u origin main
  *** -u flag is short for --set-upstream. Here's what it does:

    -u or --set-upstream:
  This flag sets the upstream (tracking) reference for the current branch.

   After using -u, Git remembers the remote (origin) and branch (main or master) you pushed to, so in the future, you can simply run git push or git pull without specifying the remote and branch again.
