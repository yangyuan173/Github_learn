
---------------------------------------

List of important git commands. Text within < > should be replaced by your own information.

---------------------------------------
- Download and install [Github Desktop](https://desktop.github.com/). 

- Create a local repo:

        cd <path-to-repo>
        git init

  Then this folder is your local repository. You can track all your changes.
  
- If we want to link this local repo to your github account, then go to your github account, creat a new "empty" repo. Then copy the link.

       cd <path-to-repo>
       git remote add origin <URL-to-remote-repo>

  You probably need to type in your github password for doing this.
  
- If you have a remote repo, then just clone it to your local computer:
      
       git clone <URL-to-remote-repo>
       
- Create new files, then add them to your repo:

        git add <file1> <file2>
 
   Or add all new files:
 
        git add -A
 
- Delete files, then stage the deletion for next commit:
 
        git rm <file1> <file2>

- Check your local repo status:

        git status

  If there are any changes that have been staged (add/rm), commit all changes:

        git commit -m "Your Message"
  Commit some changes without staging:

        git commit -a
  then edit your commit file.

- Check your local repo status:

      git status
    
  If all changes are commited and your local repo is ahead of your remote repo, then update your remote repo:

      git push -u origin master
    
- Check you remote repo status:

      git remote show origin
    
  If your local repo is out of date, then update your local repo:

      git pull
      
      
--------------------------------
# Advanced commands

- If you want to go back to a previous version, check the log file first:
      
      git log
  then fork the old version as a new branch:
      
      git checkout -b newBranch oldCommitHashOrBranchName
      
 - Delete a local branch:
 
       git branch -d newBranch
   or: 
       
       git branch -D newBranch
       
- To delete a remote branch you can use the following command:

       git push <remote_name> --delete <branch_name>
       
       

