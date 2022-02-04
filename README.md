# ansible-role-hermes
Ansible Roles to install a hermes system in a Debian 11 (bullseye), 
requires hermes user created on the host and ssh and sudo installed on the hosts

# Sections:
## Playbooks
The playbooks are on root folder and is directly related with the networks associated:
- achuar
- kaninde
- kurupira

## Basic instructions
### examples 
- To run some tags
'''ansible-playbook install.yml -i inventory --tags "web-api,web-gui"'''

- To run all without some tags:
'''ansible-playbook install.yml -i inventory --skip-tags "vara"'''

### To use encrypted vars on inventory or group_vars

'''ansible-playbook install.yml -i inventory --ask-vault-pass'''