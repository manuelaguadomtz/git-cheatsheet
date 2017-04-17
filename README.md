# Git cheatsheet

> Git features that have proven to be very useful for developers

## Configurations

git config --global user.name "John Doe"  # To set the global username

git config --global user.mail "johndoe@domain.com"  # To set the global user email

git config --local user.name "John Doe"  # To set the local username

git config --local user.mail "johndoe@domain.com"  # To set the local user email

git config --global --unset-all user.name  # To unset things

git config --global --list  # To list global configurations

git config --global --replace-all user.name "New User Name"  # To replace configurations

git config core.fileMode false  # To ignore file mode changes (i.e file permissions)

git config --global core.autocrlf true  # To ignore new line character differences between systems (windows-linux)

## Working with remotes

git remote  # List all the configured remote repositories

git remote rm <remote>  # Remove a remote repository

git push <remote> --all # To push all your branches.

git push <remote> --tags # To push all your tags:

## Working with Branches

git branch  # List all the branches

git checkout <branch>  # Make a switch to a specified branch

git branch -d <branch>  # Deleting specified branch

git branch -u <remote>/<branch> # To track a remote branch

## Reverting to previous states

### Files

`# showing file snapshot at specific commit`
git show <commit-sha>:relative/path/to/file/inside/repo

`# saving file snapshot at specific commit`
git show <commit-sha>:relative/path/to/file/inside/repo > /new/path/to/file/content/at/selected/commit

## Miscelaneous

git log -1  # Showing last commit

git log --decorate --graph -5   # To show the current local history (-5 last five commits)

