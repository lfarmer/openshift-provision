# Ansible with Vagrant/ JBoss and Oracle

##  Vagrant - CentOs7

Vagrant is used to allow users to quickly build / destroy and re-build environments with ease.  
For more information on Vagrant please check out their [Vagrant website](https://www.vagrantup.com/)

## Getting started

*N.B. Running Ansible on Windows is not currently supported* 

### Set up steps

1. [Install Vagrant.](https://www.vagrantup.com/docs/installation/)
2. Run `$vagrant up` from project root.
3. Make a note of port mappings - these could of changed if conflicts are discovered.
4. [Install Ansible.](http://docs.ansible.com/ansible/intro_installation.html) 
6. Run `$ ansible-playbook -i hosts --private-key .vagrant/machines/default/virtualbox/private_key single.yml` from project root
   