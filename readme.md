---------------------------------------
This is a document to introduce some important git commands. Text within < > should be replaced for your own needs.

---------------------------------------
- Download Git or Github Desktop.

- Create a local repo:

        cd <path-to-repo>
        git init

  Then this folder is your local repository. You can track all your changes.
- Create new files, then add them to your repo:

        git add <file1> <file2>
 
   Or add all new files:
 
        git add -A
 
- Delete files, then stage the deletion for next commit:
 
       git rm <file1> <file2>

- Check your local repo status:

        git status

  If there are any changes, commit all changes:

        git commit -m "Your Message"
  or only commit some changes:

        git commit -a
  then edit your commit file.

- If we want to link this local repo to your github account, then go to your github account, creat a new repo. Then copy the url.

      cd <path-to-repo>
      git remote add origin <https://github.com/yangyuan173/Github_learn.git>

  You probably need to type in your github password for doing this.

- Check your local repo status:

      git status
    
  If all changes are commited and your local repo is ahead of your remote repo, then update your remote repo:

      git push -u origin master
    
- Check you remote repo status:

      git remote show origin
    
  If your local repo is out of date, then update your local repo:

      git pull


