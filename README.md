# mounting-network-drives-for-user

This is a guide about how to mount network drives in folders under /home/{user}/{fldrName}

1. Create a file called .mount in the home folder of the user based on the mount file in this git.
2. Create a file called .smb.cred following the normal smb credential file rules.
3. Create a file matching the user-mount file in this git and place it somewhere apprpriate [e.g. /usr/local/bin/]
4. Amend /etc/rc.local adding "python3 /usr/local/bin/user-mount", I suggest toward the end.

reboot and the network shared drives should be there mounted in the folders in the user's home folder
