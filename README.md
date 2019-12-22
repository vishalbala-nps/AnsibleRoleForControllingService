# AnsibileRoleForControllingService
An Ansible role for controlling a service
## Overview
This is an Ansible role for starting, stopping or restarting a service in Fedora. (though it may work on other linux distributions)
## Requirements
 - You need to have a user on the remote server configured with passwordless sudo. 
 - The remote server should also have ssh configured based on Ansible's requirements
## How to Use
 - Begin by first cloning the repository with the command:  `git clone https://github.com/vishalbala-nps/AnsibleRoleForControllingService`
- Change the IP Address of the remote server in the inventory file and change the remote server username in the test.yml file
- Run the role by typing the command `ansible-playbook -i ./inventory play.yml`
- When running the role, it will ask you details like the service name and the action (start, stop or restart) 
