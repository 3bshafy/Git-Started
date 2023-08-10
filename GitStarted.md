# GitStarted

## What is Git ?

Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

> So basically Git was made to elimante the need for a scenario like  
> were you create these kind of files Finalproject, FinalFinalproject,  
> FinalProject v3.0 after each and every change done  to your code.

## Helping Commands

To start using Git we first need to know some helping commands that help us manipulate the files like pros,
the main purpose of this repo is to be able to use Git like true masters do not in the ordinary lame way.
That also includes manipulating files, renaming them or even changing the working directory. Will it take 
more time to do that in bash command line? ofcourse it will!!! But you'll look awesome man it's the goal...

### 1-"cd" Command

```sh
$cd [directory] 
```
> Before diving into usage of cd command, it is important to understand  
> what it does. cd command is a built-in command in Bash that is used to  
> change current working directory. When you execute cd command, you are  
> telling shell to change directory that you are currently working in.  
> Here, directory refers to directory that you want to change to. If you  
> do not specify a directory, cd command will take you to your home  
> directory by default.

| Argument | Purpose |
| -------- | ------- |
| No Arguments | Takes you to home directory |
| - | Takes you back to previous working directory |
| dirname | Takes you to specified directory |

`Note: if the directory name contains spaces put it between double qoutes ("") so it is treated as one argument`

## Git Commands (***The Real Deal***)

### Creating A Git Directory

Now we got a project file that we need to apply version control for, In other words use Git. first of all we need to [Install Git][Git] on our device.  
We're gonna be interacting with a commandline type of an interface that we can access by right-clicking anywhere and choosing `Git Bash Here`, then we'll use the first helping command, our deer `cd` to change our working directory to the project file we want to initilize as git repo.

1. **git init**

```sh
$ git init
```
> The git init command creates a new Git repository. It can be used to convert an existing, unversioned  
> project to a Git repository or initialize a new, empty repository. Most other Git commands are not  
> available outside of an initialized repository, so this is usually the first command you'll run in  
> a new project.

> Executing git init creates a .git subdirectory in the current working directory, which contains all  
> of the necessary Git metadata for the new repository. This metadata includes subdirectories for objects,  
> refs, and template files.

After creating your local repo in previous step now we need some sort of cloud based server so we can share and store our work and the saviour of the day is our beloved GitHub, GitHub is a website and cloud-based service that helps developers store and manage their code, as well as track and control changes to their code.
So i assume that we already have a GitHub account, we create the repo on website and then at the setaup part we will find a link, don't miss it as we're gonna need it.

2. **git remote add origin**

```sh
$ git remote add origin [remote_url]
```
> Now is the time to connect our local repo to GitHub, remember that link i mention above? will it is  
> that remote-url, so we copy it then we run the command and voilaa!! now we have a GitHub repo and we  
> are ready for the real deal. 

### Manipulating Your Repo(***Add/commit/Push/Pull/etc..***) 

- **The Sequence of Adding Your Changes to the Repo**

Let's say you worked for a while on your project and wrote/deleted code and/or added new files or made any modification to the working directory, then all these modifications are still local you need to upload these changes to the repo on GitHub. Then you'll probably use the following sequence in most of the cases.

`Note: the following sequence may vary according to the branch/nature of the repo and other factors but this is the most common procedure where you check you're on the latest version, modify localy, add changes, commit and then push`

```c
// Make sure you're on the latest version of your project before working on it 
$ git pull

// List which files are staged, unstaged, and untracked. 
$ git status

// The git add command adds a change in the working directory to the staging area. 
// It tells Git that you want to include updates to a particular file in the next commit.
$ git add .

// Takes the staged snapshot and commits it to the project history. 
// Combined with git add, this defines the basic workflow for all Git users.
$ git commit -m"commit_message"

// is utilized to send the committed changes to remote repositories for collaboration.
// This enables other team members to access a set of saved changes.
$ git push
```
`Note if it is your first push you should use `$ git push --set-upstream origin main` instead`

[Git]:<https://git-scm.com/downloads>