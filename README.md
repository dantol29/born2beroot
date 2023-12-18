# born2beroot
Setting up a secure and minimalistic virtual machine running a Linux distribution

## Managing users
**sudo adduser name** - add user

**sudo deluser name** - delete user

**sudo addgroup name** - add group

**sudo delgroup name** - delete group

**sudo adduser username groupname** - add user to the group

**getent group name** - check specific group

**getent group users** - all users

**getent group** - all groups and users

**sudo chage -l name** - password expire rules

## Firewall and SSH
**sudo ufw status** - check opened ports and firewall status

**sudo uwf allow number** - open a port

**sudo ufw delete number** - close a port

**sudo systemctl status ssh** - check ssh status

## How to connect using SSH

1. If you have this kind of IP adress 10.0.2.15 you have to connect with NAT (Host 4243, Guest 4242)

   ssh username@localhost -p 4243

2. If you have this type of IP adress 10.12.250.143 you can connect with Bridged Adaptor

   ssh username@10.12.250.143 -p 4242
## Understanding what is happening
**APPArmor** - security model in Kernel that allows sys admin to restrict capabilities of a program

**LVM** - storage managment solution. Managind of disk drives and partitions

**UFW** - policies for incoming and outgoing traffic
