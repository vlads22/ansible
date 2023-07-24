# Objective of the project
Demonstrate possible workflow that uses Ansible with two remote hosts.

# Steps taken to create the project:
- Generate SSH key and copy the public key to the two servers
- Create the `inventory` file containing the 2 remote servers.
- Create the `ansible.cfg` file containing the default inventory and SSH private key location.
- Use `ansible all -m gather_facts --limit <host name>` to gather information about the hosts.
	- `ansible all -m gather_facts --limit <host name> | grep ansible_distribution` to focus on the distribution.
- Create the first playbook: `install_apache.yml` that will install apache2 on the 2 servers.
