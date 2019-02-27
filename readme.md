---------------------------------------
Download Git or Github Desktop.

Create a local repo:

    cd path-to-repo
    git init

Then this folder is your local repository. You can track all your changes.
Write some code, then add it to your repo:

    git add

If we want to link this local repo to your github account, then go to your github account, creat a new repo. Then copy the url.

    cd path-to-repo
    git remote add origin https://github.com/yangyuan173/Github_learn.git 

You probably need to type in your github password for doing this.

Check your status:

    git status
    
If your local repo is ahead of your remote repo, then:

    git push -u origin master
    
If your local repo is outdated, then:

    git pull


