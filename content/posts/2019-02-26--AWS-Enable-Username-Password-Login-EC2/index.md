---
title: Enable Username Password Login EC2
category: "AWS"
cover: AWS_Simple_Icons_AWS_Cloud.svg.png
author: Mudit Porwal
---
# Enable Username Password Amazon EC2 Instances
Sometimes you need username and password based access to EC2. It could be either your team accessing the servers or some plugin from your IDE that works only with username and password.

Reference : [How can i create a user with password in EC2 instance?](https://serverfault.com/questions/451119/how-can-i-create-a-user-with-password-in-ec2-instance)
## Enable Username Password for EC2
You need to enable password authentication first before setting a user password. To do that:

    Edit the sshd configuration file /etc/ssh/sshd_config as root.
    
    Find the parameter PasswordAuthentication. Make sure it's uncommented and set to yes.
    
    Save the file and exit. Restart ssh service for this to take effect.

[How to restart ssh service](https://www.cyberciti.biz/faq/howto-restart-ssh/) or just restart the EC2 Instance

Now, using the following command to set the user password:

    passwd UserName

That's it! You should try to login now without the key file. 
