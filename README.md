# Git Walkthrough for COP3502

## Installing Git
### On Mac
Install Git Bash binary or Install via Homebrew
>Homebrew will require installing homebrew first

*If using Git Binary Installer*
1. Download the executable via [sourceforge.net](https://sourceforge.net/projects/git-osx-installer/)
2. Run the installer with default configurations
>If you run into download untrusted issue, please go change system settings as follows:
>System Preferences -> Security and Privacy -> General Tab -> Select Lock icon on left bottom corner -> Allow app from unidentified developer

*If using Xcode*
1. Install Homebrew by running the following command in the terminal:
`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
2. Install git via Homebrew by running `brew install git`



### On Windows
1. Install Git Bash via [git-scm.com](https://git-scm.com/download/win)
2. Download the correct executable for your system
2. Run the executable
3. Default configurations are fine

## Creating Github Account

## First Commit
### On Mac
1. Navigate to the folder where you want to create your repo
2. On the command tab, go to Finder -> Services -> New Terminal at Folder
>If you do not see this option, you might need to add this option in System Preferences, follow that [here](#add-new-terminal-service)

### On Windows
1. Open folder of file you want to add to repo in File Explorer
2. Right-click on the empty space, choose Git Bash from the options
3. Initialize a local git repository via `git init`
3. Add the files that you want either via `git add [FILENAME]` or `git add *`
4. Commit the files with message about your commit `git commit -m "[YOUR MESSAGE]`
>[OPTIONAL] The industry standard is to change branch from master to main here
>If you choose this, an additional command of `git branch -M main`
>If you get author unknown error, please follow the set author section [here](#setting-author)
5. Link the remote repository with your local repository `git remote add origin [HTTP Link]`
>HTTP Link can be copied on your Code Tab on Github either under Green Code Button or just as the link
6. Push your local repository to your remote repository `git push -u origin master`
>[OPTIONAL] If you use this option for main branch, the command is `git push -u origin main`


## Second Commit
### On Mac

### On Windows
1. Open Git Bash if you do not already have it open
2. Add the files that you have changed via `git add [FILENAME]` or `git add *`
3. Commit the files with a message via `git commit -m "[YOUR MESSAGE]"`
4. Push your files onto the remote repository `git push`

## Adding contributors

1. Go to `Settings` Tab
>This should be on the same row as Code Tab
2. Got to `Manage Access`
3. Under `Manage Access`, click on `Add people`
4. Add the Github username of your TA


## FAQ

### Setting author
If this is the first time using git or you are having trouble with author, please run the following commands with your name and email tied to the GitHub Account.

1. Set your name via `git config --global user.name "[YOUR NAME]"`
2. Set your email via `git config --global user.email "[YOUREMAIL@DOMAIN]`

### Add New Terminal Service
This will add the service option for New Terminal Window on Mac.

1. System Preferences -> Keyboard -> Shortcuts Tab -> Services
2. Check New Terminal at Folder *AND* New Terminal Tab at Folder