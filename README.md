# Ansible Wordpress Playbook
 
This playbook is for setting up version 4.9.x of the Wordpress on a local server. 

## Notes and requirements

 - The playbook was built and tested on Ubuntu 14.04 VMs, for Wordpress versions 4.9.x
 - You will need Ansible installed and running
 - Playbook is currently configured to set up the Wordpress for server open source Content Management System (CMS). 
 
 ## Instructions
 
 1. Edit your Ansible hosts file ('/etc/ansible/hosts') and add an 'wordpress' entry for the server you wish to install Wordpress on. You can of course name the host any way you want, this is just an example. 
 2. Verify connectivity to the wordpress server.
 3. In the terminal on the machine hosting Ansible, clone this repo.
 4. Cd into the directory, and run:
 `ansible-playbook -i hosts playbook.yml`
 
 The plays in the playbook will run on the target server, installing ELK and the specified beats shippers. 
 
[playbook.yml]: https://github.com/smarthardwork/Project2/playbook.yml
