### Git Version Control 
A version control system is a software that tracks changes to a file or set of files over time so that you can recall specific versions later. It also allows you to work together with other programmers or developers. The version control system is a collection of software tools that help a team to manage changes in a source code. It uses a special kind of database to keep track of every modification to the code. 

#### What is Git?
Git is an open-source distributed version control system. It is designed to handle minor to major projects with high speed and efficiency. It is developed to co-ordinate the work among the developers. The version control allows us to track and work together with our team members at the same workspace.

Git is foundation of many services like GitHub and GitLab, but we can use Git without using any other Git services. Git can be used privately and publicly.

#### Major benefits of Git are:

##### Saves Time
Git is lightning fast technology. Each command takes only a few seconds to execute so we can save a lot of time as compared to login to a GitHub account and find out its features.

##### Offline Working
One of the most important benefits of Git is that it supports offline working. If we are facing internet connectivity issues, it will not affect our work. In Git, we can do almost everything locally. Comparatively, other CVS like SVN is limited and prefer the connection with the central repository.

##### Undo Mistakes
One additional benefit of Git is we can Undo mistakes. Sometimes the undo can be a savior option for us. Git provides the undo option for almost everything.

##### Track the Changes
Git facilitates with some exciting features such as Diff, Log, and Status, which allows us to track changes so we can check the status, compare our files or branches.

### Instructions for configuration

#### Configuring Git

Now that we have install git lets config our environment. To configure we use the git config command

Git supports a command called git config that lets you get and set configuration variables that control all facets of how Git looks and operates. It is used to set Git configuration values on a global or local project level.

Setting user.name and user.email are the necessary configuration options as your name and email will show up in your commit messages.



### Setting username

The username is used by the Git for each commit.

$ git config --global user.name "Firstname Lastname"

Setting email id 

The Git uses this email id for each commit.

$ git config --global user.email "test@mydomain.com"

Other configuration options include:

Setting editor

You can set the default text editor when Git needs you to type in a message. If you have not selected any of the editors, Git will use your default system's editor.

To select a different text editor, such as Vim,

$ git config --global core.editor Vim

Checking Your Settings

You can check your configuration settings; you can use the git config --list command to list all the settings that Git can find at that point.

$ git config -list.

Colored output

You can customize your Git output to view a personalized color theme. The git config can be used to set these color themes.

Color.ui

$ Git config -global color.ui true  

The default value of color.ui is set as auto, which will apply colors to the immediate terminal output stream. You can set the colour value as true, false, auto, and always.

### Git configuration levels
The git config command can accept arguments to specify the configuration level. The following configuration levels are available in the Git config.

--local
It is the default level in Git. Git config will write to a local level if no configuration option is given. Local configuration values are stored in .git/config directory as a file.

--global
The global level configuration is user-specific configuration. User-specific means, it is applied to an individual operating system user. Global configuration values are stored in a user's home directory. 

--system
The system-level configuration is applied across an entire system. The entire system means all users on an operating system and all repositories. The system-level configuration file stores in a gitconfig file off the system directory. 

The order of priority of the Git config is local, global, and system, respectively. It means when looking for a configuration value, Git will start at the local level and bubble up to the system level.

### Git Tools
To explore the robust functionality of Git, we should learn about git tools. Git comes with some tools like Git Bash, Git GUI to provide the interface between machine and user. It supports inbuilt as well as third-party tools.

Git comes with built-in GUI tools like git bash, git-gui, and gitk for committing and browsing. It also supports several third-party tools for users looking for platform-specific experience.

Git Package Tools
Git provides powerful functionality tools such as commands, command line, Git GUI. Let's have a glimpse of some essential package tools.

GitBash
Git Bash is an application for the Windows environment. It is used as Git command line for windows. Git Bash provides an emulation layer for a Git command-line experience. Bash is an abbreviation of Bourne Again Shell. Git package installer contains Bash, bash utilities, and Git on a Windows operating system.

Bash is a standard default shell on Linux and macOS. A shell is a terminal application which is used to create an interface with an operating system through commands.

By default, Git Windows package contains the Git Bash tool. We can access it by right-click on a folder in Windows Explorer.

Git Bash Commands
Git Bash comes with some additional commands that are stored in the /usr/bin directory of the Git Bash emulation. Git Bash can provide a robust shell experience on Windows. Git Bash comes with some essential shell commands like Ssh, scp, cat, find.

Git Bash also includes the full set of Git core commands like git clone, git commit, git checkout, git push, and more.

Git GUI
Git GUI is a powerful alternative to Git BASH. It offers a graphical version of the Git command line function, as well as comprehensive visual diff tools. We can access it by simply right click on a folder or location in windows explorer. Also, we can access it through the command line by typing below command.

$ git gui  

A pop-up window will open as Git gui tool. The Git GUI's interface looks like as:




### Basic Git Command
Git clone command
This command is used to make a copy of a repository from an existing URL. If I want a local copy of my repository from GitHub, this command allows creating a local copy of that repository on your local directory from the repository URL.

Syntax
$ git clone URL

Git add command
This command is used to add one or more files to staging (Index) area.

Syntax
To add one file

$ git add Filename  

To add more than one file

$ git add*

Git commit command
Commit command is used in two scenarios. They are as follows.

Git commit -m

This command changes the head. It records or snapshots the file permanently in the version history with a message.

Syntax

$ git commit -m " Commit Message"  

Git commit -a

This command commits any files added in the repository with git add and also commits any files you've changed since then.

Syntax

$ git commit -a

Git status command
The status command is used to display the state of the working directory and the staging area. It allows you to see which changes have been staged, which haven't, and which files aren?t being tracked by Git. It does not show you any information about the committed project history. For this, you need to use the git log. It also lists the files that you've changed and those you still need to add or commit.

Syntax

$ git status

Git push Command
It is used to upload local repository content to a remote repository. Pushing is an act of transfer commits from your local repository to a remote repo. It's the complement to git fetch, but whereas fetching imports commits to local branches on comparatively pushing exports commits to remote branches. Remote branches are configured by using the git remote command. Pushing is capable of overwriting changes, and caution should be taken when pushing.

Git push command can be used as follows.

Git push origin master

This command sends the changes made on the master branch, to your remote repository.

Syntax

$ git push [variable name] master  

Git push -all
This command pushes all the branches to the server repository.

Syntax

$ git push --all

Git pull command
Pull command is used to receive data from GitHub. It fetches and merges changes on the remote server to your working directory.

Syntax

$ git pull URL  

Git Branch Command
This command lists all the branches available in the repository.

Syntax

$ git branch

Git Merge Command
This command is used to merge the specified branch?s history into the current branch.

Syntax

$ git merge BranchName

Git log Command
This command is used to check the commit history.

Syntax

$ git log

By default, if no argument passed, Git log shows the most recent commits first. We can limit the number of log entries displayed by passing a number as an option, such as -3 to show only the last three entries.

$ git log -3 

Git Clone Branch
Git allows making a copy of only a particular branch from a repository. You can make a directory for the individual branch by using the git clone command. To make a clone branch, you need to specify the branch name with -b command. Below is the syntax of the command to clone the specific git branch:

$ git clone -b <Branch name><Repository URL>

Git Fork
A fork is a rough copy of a repository. Forking a repository allows you to freely test and debug with changes without affecting the original project. One of the excessive use of forking is to propose changes for bug fixing. To resolve an issue for a bug that you found, you can:

Fork the repository.
Make the fix.
Forward a pull request to the project owner.
Forking is not a Git function; it is a feature of Git service like GitHub.

Generally, forking a repository allows us to experiment on the project without affecting the original project. Following are the reasons for forking the repository:

How to Fork a Repository on GitHub?
The forking and branching are excellent ways to contribute to an open-source project. These two features of Git allow the enhanced collaboration on the projects.

Forking is a safe way to contribute. It allows us to make a rough copy of the project. We can freely experiment on the project. After the final version of the project, we can create a pull request for merging.

It is a straight-forward process. Steps for forking the repository are as follows:

Login to the GitHub account.
Find the GitHub repository which you want to fork.
Click the Fork button on the upper right side of the repository's page.

### Inspect and Undo changes

Git log
The advantage of a version control system is that it records changes. These records allow us to retrieve the data like commits, figuring out bugs, updates. But, all of this history will be useless if we cannot navigate it. At this point, we need the git log command.

Git log is a utility tool to review and read a history of everything that happens to a repository. Multiple options can be used with a git log to make history more specific.

Generally, the git log is a record of commits. A git log contains the following data:

A commit hash, which is a 40-character checksum data generated by SHA (Secure Hash Algorithm) algorithm. It is a unique number.
Commit Author metadata: The information of authors such as author name and email.
Commit Date metadata: It's a date timestamp for the time of the commit.
Commit title/message: It is the overview of the commit given in the commit message.
Basic Git log
Git log command is one of the most usual commands of git. It is the most useful command for Git. Every time you need to check the history, you have to use the git log command. The basic git log command will display the most recent commits and the status of the head. It will use as:

$ git log 

The above command is listing all the recent commits. Each commit contains some unique sha-id, which is generated by the SHA algorithm. It also includes the date, time, author, and some additional details.

Git Log Stat
The log command displays the files that have been modified. It also shows the number of lines and a summary line of the total records that have been updated.

Generally, we can say that the stat option is used to display

the modified files,
The number of lines that have been added or removed
A summary line of the total number of records changed
The lines that have been added or removed.
It will be used as follows:

$ git log --stat

Git log P or Patch

The git log patch command displays the files that have been modified. It also shows the location of the added, removed, and updated lines.

It will be used as:

$ git log --patch Or $ git log -p

Generally, we can say that the --patch flag is used to display:

Modified files
The location of the lines that you added or removed
Specific changes that have been made.
Git Checkout
In Git, the term checkout is used for the act of switching between different versions of a target entity. The git checkout command is used to switch between branches in a repository. Be careful with your staged files and commits when switching between branches.

Image Git Checkout

The git checkout command operates upon three different entities which are files, commits, and branches. Sometimes this command can be dangerous because there is no undo option available on this command.

It checks the branches and updates the files in the working directory to match the version already available in that branch, and it forwards the updates to Git to save all new commit in that branch.

Operations on Git Checkout
We can perform many operations by git checkout command like the switch to a specific branch, create a new branch, checkout a remote branch, and more. The git branch and git checkout commands can be integrated.

Checkout Branch
To switch between branches, use the below command.

$ git checkout <branchname>

Create and Switch Branch

The git checkout commands let you create and switch to a new branch. You can not only create a new branch but also switch it simultaneously by a single command. The git checkout -b option is a convenience flag that performs run git branch <new-branch>operation before running git checkout <new-branch>.

$ git checkout -b <branchname>

Checkout Remote Branch

Git allows you to check out a remote branch by git checkout command. It is a way for a programmer to access the work of a colleague or collaborator for review and collaboration. Each remote repository contains its own set of branches. So, to check out a remote branch, you have first to fetch the contents of the branch.

$ git checkout <remotebranch>

#### Collaborating
Collaborating in git git refers to sharing on code among several developers. We will look at code sharing is handled in Git.We will discuss major collaboration operations in Git.  Our main focus will be on Git fetch, Git pull and Git Push.

Git Fetch
Git "fetch" Downloads commits, objects and refs from another repository. It fetches branches and tags from one or more repositories. It holds repositories along with the objects that are necessary to complete their histories to keep updated remote-tracking branches.

The "git fetch" command is used to pull the updates from remote-tracking branches.

Git Pull / Pull Request
The term pull is used to receive data from GitHub. It fetches and merges changes from the remote server to your working directory. The git pull command is used to pull a repository.


```python

```
