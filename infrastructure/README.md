# Infrastructure

## Setup SFTP user

```
sudo useradd {user}
sudo su {user} -
ssh-keygen
chmod 700 .ssh
mv .ssh/id_rsa.pub .ssh/authorized_keys
chmod 600 .ssh/authorized_keys
cat .ssh/id_rsa # Save the string on your local
vim /etc/ssh/sshd_config

# Add following code
# Match User {user}
# ChrootDirectory {path to root for this user}
# ForceCommand internal-sftp -u 002

sudo service sshd restart
```
