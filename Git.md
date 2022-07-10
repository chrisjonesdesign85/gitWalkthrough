# Git
On Windows you should use Git Bash on Mac/Linux the command line terminal will work for this.

Before we dive into git I think it is important to know the basic Linux commands to be able to navigate around the file system, how to create and edit files etc.

`pwd` print working directory. This will show us the current working directory.

`ls` This will list all the files and folders in the current directory.
 
 `ll` or `ls -l` will list the files with more detail.
 
`mkdir dirName` create a new directory. (dirName = your file name)

`cd ..` will go back to the previous directory.

`cd dirName` change directory. (dirName = the folder you want to navigate to.)

`touch fileName` create a new file (fileName = your file name)
such as `touch index.html`

I would create the folder and create all the necessary files such as: `index.html, styles.css and, main.js or app.js`. 

You can create all the files in one command as follows:
`touch index.html styles.css main.js`

`git init` This will tell Git to get ready to start watching your files for every change that occurs.

`git log` This will show the git history of all the commits.

`git log --author="name"` This will only show commits by a specific person.

`git status`  This will show current changes to files and folders.

`git branch` will show you what branch you are on currently.

`git checkout -b name-of-branch` This will create a new branch separate from the `main` or `master` branch, where `name-of-branch` is the name you have entered.

You are now working on your own branch. It is important to keep your work separate from the main or master branch.

Once you have made some progress it's time to make a commit.

`git add .`  This will add all files to the commit.

`git add file-name` This will add specific files that have been created or modified. *`file-name` the file name you have chosen*

`git commit -m "This is a coment about the commit"` 
This will make a new commit to the branch you are on. Be sure to leave a comment as to what has been changed. This should have as many details as possible but keep it short. Good for in the future or when you need to revert to a previous version.


### Create a repository

 A repository is just another way to define a project being watched/tracked by Git.
 
You can click on the `+` symbol on the top right corner on the web page then choose `New repository`. Give your repo a name then scroll down and click on `Create repository`.
 
Before we "add" and "commit" or files, we need to understand the stages of a file being tracked by Git.

#### Committed state
A file is in the `committed` state when all the changes made to the file have been saved in the local repo. Files in the committed stage are files ready to be pushed to the remote repo(on GitHub).

#### Modified state
A file in the `modified` state has some changes made to it but it's not yet saved.
This means that the state of the file has been altered from its previous state in the committed state.

#### Staged state
A file in the `staged` state means it is ready to e committed. In this state, all necessary changes have been made so the next step is to move the file to the commit state.

You can understand this better by imagining Git as a camera. The camera will only take a snap shot when the file reaches the commit state. After this state, the camera starts comparing changes being made to the same file with the last snapshot(this is the modified state). And when the required changes have been made, the file is staged and moved to the commit state for a new snapshot.

This might be a lot of information to take in at the moment, but do not be discouraged, it gets easier with practice.

### Fork a repo 

#### What is a fork?
A GitHub fork is a copy of a repository (repo) that is in your account and not the account that you forked the data from. After forking a repo, you now have a copy of the repo. You can now edit the contents of the forked repository without affecting the original repo.

### Clone your fork

Now you should go to your main projects folder or wherever you want the project folder from GitHub to go. Use the following command to clone your repo from GitHub.

`git clone http://github.com/yourname/repo.git `

### How to push your code to the repo.
So you have opened the project in VScode and made some changes now you want to push your changes up to github.

Once you have made a commit or several, it's time to push our changes to the Repo.

### Push the commit to GitHub

`git push origin name-of-branch`
This pushes your repo from your local device to GitHub.

Now go to github and create a new `Pull Request`. make sure to switch to the branch you made your commit on.

Once you have created the new folder where you want to have the project located and you have created all the necessary files use the following command in the terminal, be sure to be in the folder that was created for the project to  open that project folder in VS Code. 

`code .`

### 4. Open project in VScode
Make sure you are in the home directory of the project and use `code .` to open the project in VSCode.
