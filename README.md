# ansible
This Repo is used for all ansible (Config mgmt tool) related activities both on push & pull activities


###Inventory : List of machine or dns names that you want ansible to be managed


### ansible_user :predefined var for userName
### ansible_password :predefined var for userPassword


modules : -m shell, -m yum , -m service

variables --should be passed by -e  
## ansible dev -i inv  -e ansible_user=centos -e ansible_password=DevOps321 -m shell -a uptime

### ansible can be executed in 2ways

1 Manual
2 Automated

### ansible-pull


ansible-pull -U urlname.git playbookName.yml -e COMPONENT=componentName


### Bloack and Rescue

Block - group oof tasks
Rescue - executed if any of the taks in the blocks fail

### Ansible -Dry run

ansible-playbook robot-dryrun.yaml -e COMPONENT=mongodb -e ansible_user=centos -e ansible_password=DevOps321 -e ENV=qa


### Playboook

Playbook -- list of plays
Play     -- list of tasks
Task     -- list of actions 

