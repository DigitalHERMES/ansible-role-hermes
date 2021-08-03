# hermes-install


# inventory / host vars

## /etc/ansible/hosts 
content:
´´´hermes ansible_port=22 ansible_host=192.168.0.21 ansible_user=hermes ´´

## /etc/ansible/host_vars/hermes
    password_api: very_secret_key 
    password_admin: caduceu
    webpub_path: /var/www
    # check this !
    install_system_packages: true
    install_wine: true
    install_uuardop_path: /tmp/build
    build_path: /home/hermes/install
    hostname: ansible_hostname
    www_group: www-data
