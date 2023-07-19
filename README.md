# Objective of the project
Demonstrate the use of Ansible with two remote Ubuntu servers.

# Steps taken to create the project:
- Generate SSH key and copy the public key to the two servers
- Create the `inventory` file containing the 2 remote servers.
- Create the `ansible.cfg` file containing the default inventory and SSH private key location.
- Create the first playbook: `install_apache.yml` that will install apache2 on the 2 servers.
