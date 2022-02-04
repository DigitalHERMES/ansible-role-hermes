# ansible-role-hermes
Ansible Roles to install a hermes system in a Debian 11 (bullseye), requires creation of a user in sudo groupo, ssh and sudo installed, update or create hosts networks inside 

# Sections:
## Playbooks
The main playbook is the install in root folder

## Basic instructions
### examples 
- To run some tags
'''ansible-playbook install.yml -i inventory --tags "web-api,web-gui"'''

- To run all without some tags:
'''ansible-playbook install.yml -i inventory --skip-tags "vara"'''

### To use encrypted vars on inventory or group_vars

'''ansible-playbook install.yml -i inventory --ask-vault-pass'''