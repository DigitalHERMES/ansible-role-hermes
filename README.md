## ansible-role-hermes
ansible-roles to install a hermes system in a Debian 11 (bullseye)

## Playbooks
The playbooks are on root folder and is directly related with the networks associated:
- achuar
- kaninde
- kurupira

## Basic instructions
- To run some tags
'''ansible-playbook kurupira.yml -i inventory --tags "web-api,web-gui"'''

- To run all without some tags:
'''ansible-playbook kurupira.yml -i inventory --skip-tags "vara"'''

## To use encrypted vars on inventory or group_vars

'''ansible-playbook kurupira.yml -i inventory --ask-vault-pass'''

