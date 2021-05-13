# SSH NOTES

### Key generation
 
 > ssh-keygen

 > ssh-keygen -t rsa

</br>

 ### Add new key

 > ssh-add /home/username/.ssh/id_rsa_github.pub

if you get a message about auth run this and try again

> eval `ssh-agent -s`

</br>

### Run this command to skip authentication using password / pem file every time u connect through ssh

> sudo cat ~/.ssh/id_rsa.pub | ssh -i "servername" "mkdir -p ~/.ssh && chmod 700 ~/.ssh && cat >>  ~/.ssh/authorized_keys"

