# Git cheatsheet

> Git features that have proven to be very useful for developers

## Configurations

`# set the global username`

```bash
git config --global user.name "John Doe"
```

`# set the global user email`

```bash
git config --global user.mail "johndoe@domain.com"
```

`# set the local username`

```bash
git config --local user.name "John Doe"
```

`# set the local user email`

```bash
git config --local user.mail "johndoe@domain.com"
```

`# to unset a given configuration`

```bash
git config --global --unset-all user.name

```

`# to list global configurations`

```bash
git config --global --list
```

`# to replace configurations`

```bash
git config --global --replace-all user.name "New User Name"
```

`# to ignore file mode changes (i.e file permissions)`

```bash
git config core.fileMode false
```

`# to ignore new line character differences between systems (windows-linux)`

```bash
git config --global core.autocrlf true
```

## Working with remotes

`# list all the configured remote repositories`

```bash
git remote
```

`# remove a remote address for the repository`

```bash
git remote rm <remote>
```

`# to push all your branches.`

```bash
git push <remote> --all
```

`# to push all your tags`

```bash
git push <remote> --tags
```

## Working with Branches

`# list all the branches`

```bash
git branch
```

`# list all the branches (local and repote branches)`

```bash
git branch --all
```

`# make a switch to a specified branch`

```bash
git checkout <branch>
```

`# deleting specified branch`

```bash
git branch -d <branch>
```

`# tracking a remote branch`

```bash
git branch -u <remote>/<branch>
```

## Reverting to previous states

### Reverting Files

`# showing file snapshot at specific commit`

```bash
git show <commit-sha>:relative/path/to/file/inside/repo
```

`# saving file snapshot at specific commit`

```bash
git show <commit-sha>:relative/path/to/file/inside/repo > /new/path/to/file/content/at/selected/commit
```

## Graph history visualization

`# showing last commit`

```bash
git log -1 
```

`# showing the current local history (-5 last five commits)`

```bash
git log --decorate --graph -5
```
