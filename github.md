# How to use GitHub!

### Install git and prepare it

If it isn't already installed, you should first install git with the command `sudo pacman -S git`.
Then in order to use _Git_, you need to set at least a name and email:

```
{ $ git config --global user.name "Astonish"
$ git config --globar user.email gatmacagit@gmail.com }
```

Then you should set the default branch name with this command:

```
{ $ git config --global init.defaultBranch main }
```

Then log-in to your Github account with `gh auth login` and authoriz it with https from the web when prompted in terminal.

### Create a folder with your repo files

First of all you should create a local directory, wherever you want in your computer to create a git repository.

> **NOTE** that _git_ and _github_ are two different things. _Git_ repository is the `.git/` folder inside a proect. This repository tracks all changed made to files in your project's hisory.
> _GitHub_ on the other hand, is a cloud service to host your _git_ project. There are also other alternatives like _Gitlab_. So, git repository **is not equal to** GitHub.
> Inside this folder put all of the files, folders..etc that you want to host.

### Start the Git repository

After doing all of the steps above succesfully, from the terminal, navigate inside your folder. To the root directory of your _Git_ repository. It is the main folder that will be uploaded to _GitHub_. From inside that folder type this comnmand:
`{ $ git init }`

### Add files to the repository

Your **local** git repository is created succesfully. By using the command `git status` you can see the tracked and untracked files. Since the repository has just been created, all the files will be untracked. Now you can add the files that you have in your folder, which you want to have included/tracked in your repository manually with the command `git add <name of the file>`. For example `git add blender.md`. Or if you want to add them all, you can type `git add .` and now if you try again the `git status` command, you will see that all of your files are in the tracked, _Changes to be committed_ list.

### Commit the files that needs to be pushed to the Git repository

Now that we have selected the files that needs to be included in our git repository, it is time to commit those files for the first time. You can use the command `git commit -m "my first commit"` to commit the files. Remember to add `-m "<some comment>"` or else the commit will fail because it has no comments or explanations.

### Create a Github repository

Go to the GitHub webpage and to the repository section of your account and click the green `NEW` button to add a new repository. There after you choose all the options you want, select the name..etc and create the repository. The page will lead you to a web page where it will explain how to push your already existing local repository in the second section. Copy and paste those three lines and your local repository will be copied to the cloud GitHub page.

### How to apply and push modifications?

Well, inside your repository, after you made the changes, add the files that you want to commit again, with always `git add <file name>` command and commit the added files with `git commit -m "<your comment>"` and finally push it with `git push -u origin main` command.
