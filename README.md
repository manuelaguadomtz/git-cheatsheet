=================Configurations=================================================================================
git config --global user.name "John Doe"  # To set the global username
git config --global user.mail "johndoe@domain.com"  # To set the global user email

git config --local user.name "John Doe"  # To set the local username
git config --local user.mail "johndoe@domain.com"  # To set the local user email

git config --global --unset-all user.name  # To unset things

git config --global --list  # To list global configurations

git config --global --replace-all user.name "New User Name"  # To replace configurations

git config core.fileMode false  # To ignore file mode changes (i.e file permissions)

git config --global core.autocrlf true  # To ignore new line character differences between systems (windows-linux)
==================================================================================================================

git branch -u origin/master


