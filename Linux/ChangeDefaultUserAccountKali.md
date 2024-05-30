# Change Default User Account on Kali Linux

Running this on a fresh Kali installation. 
Login as kali user and run these commands to add a new default user:

```
# Specify the username for your new user account
username=<your_username_here>
# Specify that the user login shell will be zsh
user_shell=$(which zsh)
# Add any group where the kali user is a member
groups=$(grep -E '\:kali$' /etc/group | cut -d ':' -f 1 | sed -z 's/\n/,/g;s/,$/\n/')
# Create the new user account
sudo useradd -m -G $groups -s $user_shell $username
# Change the new user's password
sudo passwd $username

```

Logout of kali session, login as your new user and verify permissions. If everything looks good:

* Change the kali user account password
* Disable or delete the kali user account