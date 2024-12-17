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
git add .
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
e2bc30699bbcf29881cd82521a5bd17e78e23f34
## Branches

## Remotes

## Stashing

## Merging