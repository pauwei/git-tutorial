# Git Walkthrough for COP3502

## Table of Contents
1. [Installing Git on Your Computer](#installing-git)
2. [Creating a GitHub Account](#setting-up-github)
3. [Creating your first commit](#first-commit)
4. [Updating with second commit](#second-commit)
5. [Adding Contributor to your repo](#adding-contributors)
6. [FAQ](#faq)

## Installing Git

### On Mac
Install Git Bash binary or Install via Homebrew
> Homebrew will require installing homebrew first

<br/>

If using Git Binary Installer
1. Download the executable via [sourceforge.net](https://sourceforge.net/projects/git-osx-installer/)
2. Run the installer
> If you run into download untrusted issue, please go change system settings as follows: <br/>
> System Preferences -> Security and Privacy -> General Tab -> Select Lock icon on left bottom corner -> Allow app from unidentified developer <br/>
> Default configurations are fine

<br/>

If using Homebrew
1. Install Homebrew by running the following command in the terminal: <br/>
`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
2. Install git via Homebrew by running the following command in the terminal: <br/>
`brew install git`



### On Windows
1. Install Git Bash via [git-scm.com](https://git-scm.com/download/win)
2. Download the correct executable for your system
3. Run the executable
> Default configurations are fine

## Setting up GitHub

### Creating a GitHub Account
1. Go to [github.com](https://github.com/)
2. If you do not have an account, click on the sign up button
3. Fill in the necessary information
> It is a good idea to use an username that can be easily identified you for the sake of other developers

### Creating a private repository
1. Go to [github.com](https://github.com/) homepage if you are not there.
2. Click the green button "New" to create a new repository
3. Name your repo to something specific to the code you will be uploading
4. Choose private option if required by assignment
5. Do not check any additional boxes
> If you check any additional boxes, how you initialize repository may be different

Your repo screen should like the following: <br/>
![Initial Repo Screen](https://github.com/pauwei/git-tutorial/blob/master/images/NewRepo.JPG)

## First Commit

### On Mac - Opening a Terminal Session
1. Navigate to the folder of the files you want to add in Finder
**Make sure to navigate to the folder and not just search it**, if you do not know how get to your folder, go to [here](#navigate-to-folder-mac)
2. Select the folder, then click on the settings icon for the folder
3. Click on the option "New Terminal at Folder"


### On Windows - Opening a Terminal Session
1. Open folder of file you want to add to repo in File Explorer
2. Right-click on the empty space, choose Git Bash from the options

### Running git for the first time
1. Initialize a local git repository via `git init`
2. Add the files that you want either via `git add [FILENAME]` or `git add *`
3. Commit the files with message about your commit `git commit -m "[YOUR MESSAGE]"`
> \*OPTIONAL\* The industry standard is to change branch from master to main here
> If you choose this, an additional command of `git branch -M main`

**If you get author unknown error**, please follow the set author section [here](#setting-author)
4. Link the remote repository with your local repository `git remote add origin [HTTPS Link]`
> HTTPS Link can be copied on your Code Tab on Github either under Green Code Button or just as the link
5. Push your local repository to your remote repository `git push -u origin master`
> \*OPTIONAL\* If you use this option for main branch, the command is `git push -u origin main`
6. Reload your page on GitHub to see the code you pushed


## Second Commit
### Add a change to your file
1. Either open up the file you wish to change in IntelliJ or some other editor
2. Make a slight change to show that the file has been changed

### Running git for the second time
1. Open Git Bash on Windows or Terminal on Mac if you do not already have it open
2. Add the files that you have changed via `git add [FILENAME]` or `git add *`
3. Commit the files with a message via `git commit -m "[YOUR MESSAGE]"`
4. Push your files onto the remote repository `git push`
5. Reload your page on GitHub to make sure that the new changes have been updated

## Adding contributors

1. Go to `Settings` Tab within your repository
> This should be on the same row as Code Tab
2. Got to `Manage Access`
3. Under `Manage Access`, click on `Add people`
4. Add the Github username of your TA


## FAQ

### Setting author
If this is the first time using git or you are having trouble with author, please run the following commands with your name and email tied to the GitHub Account.

1. Set your name via `git config --global user.name "[YOUR NAME]"`
2. Set your email via `git config --global user.email "[YOUREMAIL@DOMAIN]`
3. Rerun the commit command to make sure your changes were commited

### Navigate to Folder Mac
If you are using IntelliJ, these instructions should lead you to the correct folder. Otherwise, it should give you a good idea of where to start.

1. Open Finder
2. On the Taskbar at the top of your computer, select Go -> Home
3. Open the folder IdeaProjects in Finder
4. Navigate to the folder you are using