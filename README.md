# Objective of the project
Create several simple Ansible playbooks in order to update and install packages on two servers.

# Steps taken to create the project:
- Generate SSH key and copy the public key to the two servers
- Create the `inventory` file containing the 2 remote servers.
- Create the `ansible.cfg` file containing the default inventory and SSH private key location.
- Use `ansible all -m gather_facts --limit <host name>` to gather information about the hosts.
	- `ansible all -m gather_facts --limit <host name> | grep ansible_distribution` to focus on one distribution.
- Create the playbooks, example: `install_apache.yml` that will install apache2 on the 2 servers.
- Run the playbooks with, example:
	`ansible-playbook --ask-become-pass install_apache.yml`
	- and enter servers user password
	
