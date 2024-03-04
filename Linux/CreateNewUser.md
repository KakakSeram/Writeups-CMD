# Create New User

Creating new user for Linux 

## Add new username

`useradd -m [username]`

* _useradd_ command is used to create new user.
* _-m_ option to create a home directory for the new user.
* _[username]_ is specifix name to create new user.

## Set new password

`passwd [username]`

* _passwd_ command is used to create a password.
* _[username]_ is spesifix user create a new password.

## Set user group to sudo

`usermod -a -G sudo [username]`

* _usermod_ command is used to modify a user.
* _-a_ option to add.
* _-G sudo’_ means to add the user to the sudo group.
* _[username]_ is spesifix user to modify.

## Set login shell

`chsh -s /bin/bash [username]`

* _chsh_ command is used to change the login shell for a user.
* _-s_ option to add SUID.
* _/bin/bash_ is location bash shell.
* _[username]_ is set for spesifix user.