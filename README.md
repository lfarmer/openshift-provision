# Openshift provisioning with Ansible 

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
7. Clone openshift ansible github repo `$ git clone https://github.com/openshift/openshift-ansible.git`
8. `$ cd openshift-ansible`
7. Create host file for openshift configuration
8. Run openshift-ansible: `ansible-playbook -i hosts --private-key ../.vagrant/machines/default/virtualbox/private_key playbooks/byo/config.yml`
9. Go to `https://192.168.33.10:8443/console` where you should be able to log in with configured users
   