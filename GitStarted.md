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

## Git Commands (*The Real Deal*)
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



[Git]:<https://git-scm.com/downloads>