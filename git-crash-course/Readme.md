## Git Hidden Folder

there is a hidden folder called `.git` which tells us that our project is a git repo.
If we want to craete a git repo in a new project , we create the folder and initialise that repo using `git init`

```
mkdir /workspaces/temp/new-project
cd workspaces/temp/new-project
git init
touch readme.md
code Readme.md
git status
git add Readme.md
# makes changes to readme.md
git commit -a -m "add readme files"
```


## Cloning
Three ways to clone : HTTPS, SSH, GitHub CLI.
As we are using GitHub Codespaces, we will create a temporary directoryin ourworkspace
```sh
mkdir /workspace/temp
cd /workspace/temp
```

### HTTPS
```sh
git clone https://github.com/mahmudulJim/Github-Examples.git
cd Github-Examples
```

## Commits

when we want to commit code, we can write git commit which will open up the commit edit message in the editor of choice 
```sh
git commit
```
Set the global editor
```
git config --global core.editor emacs
```
When you need to modify and commit Readme.md:
```sh
code Readme.md (//here you code/modify)
git add Readme.md
git commit -m "added more exclamations"
```
in between these steps, you can command ```git status``` to see if things happening or not.

## Branches

## Remotes

## Stashing

## Merging

## Add

When we want to stage changes that will be included in the commit, We can use the . to add all possible files
```
git add Readme.md
git add .
```

## Reset

Reset allows you to move staged changes to be unstaged.
This is useful when you to revert all files not to be commited

```
git add .
git reset
```

>git reset will revert a git add.

## Status

Git status shows you what files will or will note be commited
```
git status
```

## Gitconfig File

The gitconfig file is what stores your gloabl configuration for git such as email, name, editor and more.

Showing the contents of our .gitconfig file

```sh
git config --list
```

When you first install Git on a machine you are supposed to set up your name and email.

```sh
git config --global user.name "mahmudulJim"
git config --global user.email "account@gmail.com"
```
## Log
Git log will show recent git commits to the git tree

## Push
When we want to push a repo to our remote origin

```
git push

```