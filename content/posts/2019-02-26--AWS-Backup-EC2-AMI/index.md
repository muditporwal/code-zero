---
title: Backing Up EC2 AMI/EBS
category: "AWS"
cover: AWS_Simple_Icons_AWS_Cloud.svg.png
author: Mudit Porwal
---
# Backing up Amazon EC2 Instances
There are a few ways you can backup your ec2 instances, starting from backing up your hard-disk (EBS) to taking a virtual image (AMI).A few of these steps are as put below.

Reference : [How to Back Up Amazon EC2 Instances](https://www.cloudberrylab.com/resources/blog/backup-aws-ec2-instance/)
## EC2 Backup using EBS Snapshots
One way to backup the EC2 instances is by creating snapshots of the hard-disk of your EC2. EBS - Elastic Block Storage volume is the storage space for your EC2s.
You need to stop the EC2 instances, unmount the volume and then take a snapshot of the EBS volume from the Amazon Management Console. 
On creating a snapshot you can restore back if needed under any circumstance.

## Cloning an AMI
Another way is to clone an AMI. AMI is the OS+Configuration+Data of your EC2. Normally to backup we need to stop the EC2 and then clone the AMI of the existing EC2.

Option to cloning/creating image should be under `Actions>Image>Create Image`


## Other ways to backup your Data
Please head to  [How to Back Up Amazon EC2 Instances](https://www.cloudberrylab.com/resources/blog/backup-aws-ec2-instance/)
