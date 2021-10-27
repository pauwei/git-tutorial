### Installing Git
#### On Mac
1. Install Git Bash binary

#### On Windows
1. Install Git Bash via [git-scm](https://git-scm.com/download/win)
2. Run the executable
3. Default configurations are fine

### Creating Github Account

### First Commit
#### On Mac

#### On Windows
1. Open folder of file you want to add to repo in File Explorer
2. Right-click on the empty space, choose Git Bash from the options
3. Initialize a local git repository via `git init`
3. Add the files that you want either via `git add [FILENAME]` or `git add *`
4. Commit the files with message about your commit `git commit -m "[YOUR MESSAGE]`
>[OPTIONAL] The industry standard is to change branch from master to main here
>If you choose this, an additional command of `git branch -M main`
5. Link the remote repository with your local repository `git remote add origin [HTTP Link]
>HTTP Link can be copied on your Code Tab on Github
6. Push your local repository to your remote repository `git push -u origin master`
>If you use this option for main branch, the command is `git push -u origin main`


### Second Commit

### Adding contributors

1. Go to `Settings` Tab
>This should be on the same row as Code Tab
2. Got to `Manage Access`
3. Under `Manage Access`, click on `Add people`
4. Add the Github username of your TA