# Git cheatsheet

> Git commands that have proven to be very useful for developers

## Configurations

#### Set the global username

```bash
git config --global user.name "John Doe"
```

#### Set the global user email

```bash
git config --global user.mail "johndoe@domain.com"
```

#### Set the local username

```bash
git config --local user.name "John Doe"
```

#### Set the local user email

```bash
git config --local user.mail "johndoe@domain.com"
```

#### To unset a given configuration

```bash
git config --global --unset-all user.name

```

#### To list global configurations

```bash
git config --global --list
```

#### To replace configurations

```bash
git config --global --replace-all user.name "New User Name"
```

#### To ignore file mode changes (i.e file permissions)

```bash
git config core.fileMode false
```

#### To ignore new line character differences between systems (windows-linux)

```bash
git config --global core.autocrlf true
```

#### To configure a proxy server

```bash
git config --global http.proxy http://proxyuser:proxypwd@proxy.server.com:proxy_port
```


## Working with remotes

#### List all the configured remote repositories

```bash
git remote -v
```

#### Remove a remote server

```bash
git remote rm <remote>
```

## Working with Branches

#### To push all your branches

```bash
git push <remote> --all
```

#### List all the branches

```bash
git branch
```

#### List all the branches (local and remote branches)

```bash
git branch --all
```

#### Make a switch to a specified branch

```bash
git checkout <branch>
```

#### Deleting specified branch

```bash
git branch -d <branch>
```

#### Tracking a remote branch

```bash
git branch -u <remote>/<branch>
```

#### To remove all the remote tracking branches that no longer exists

```bash
git remote prune <remote>
```

#### To remove an specific remote tracking branch

```bash
git branch -d -r <remote>/<branch>
```

#### To remove a remote branch

```bash
git push <remote> --delete <branch>
```

```bash
git push <remote> :<branch>
```


## Tagging

#### Pushing tags to the remote

```bash
git push <remote> --tags
```

#### Pushing commits and also tags to the remote

```bash
git push --follow-tags
```

#### Removing a local tag

```bash
git tag -d <tag-name>
```

#### Removing a remote tag

```bash
git push --delete <remote> tagName
```

## Reverting to previous states

### Reverting Files

#### Showing file snapshot at specific commit

```bash
git show <commit-sha>:relative/path/to/file/inside/repo
```

#### Saving file snapshot at specific commit

```bash
git show <commit-sha>:relative/path/to/file/inside/repo > /new/path/to/file/content/at/selected/commit
```

## Graph history visualization

#### Showing last commit

```bash
git log -1 
```

#### Showing the current local history (-5 last five commits)

```bash
git log --decorate --graph -5
```
