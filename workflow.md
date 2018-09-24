# common git commands

## downloading a repository to a local folder
git clone {repository-url} {optional folder_name}

## informing git that an important local file has changed
git add {file_path} {file_path}

## saving your changes in interactive mode
git commit

## saving your changes in console mode
git commit -m "short massage describing your changes"

## sending your changes to your remote repository
git push

## downloading updates from remote repository
git stash
git pull
git stash apply

# self knowledge

## listing commits
git log

## seeing the current state of your current branch
git status

## loading a previous commit and return to present
git checkout {commit-hash}

## restoring an uncommited file

## seeing if your remote url is configured correctly

- to successfully push, you must have a valid origin url: https://help.github.com/articles/adding-a-remote/

git remote -v

# working collaboratively

## downloading from others
https://help.github.com/articles/fetching-a-remote/

## uploading to others

- first thing is to create a new branch for your patch

git checkout -b my_patch

- second thing, code, add and commit your stuff
- then push your patch to a new branch inside your remote repository

git push origin my_patch

- then use a browser to navigate to your remote repository and create a pull request using the GitHub interface
