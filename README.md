# Ansible Role: LAMP
---------------------
Ansible Role that installs and configure LAMP Stack on Centos
## Requirements
In ansible master server 
* Install python:
```
amazon-linux-extras install ansible2 -y
```
* create inventory file

## Ansible Modules using
- [yum](https://docs.ansible.com/ansible/2.9/modules/yum_module.html)
- [shell](https://docs.ansible.com/ansible/2.9/modules/shell_module.html)
- [service](https://docs.ansible.com/ansible/2.9/modules/service_module.html)
- [mysql_user](https://docs.ansible.com/ansible/2.9/modules/mysql_user_module.html)
- [mysql_db](https://docs.ansible.com/ansible/2.9/modules/mysql_db_module.html)
- [get_url](https://docs.ansible.com/ansible/2.9/modules/get_url_module.html)
- [unarchive](https://docs.ansible.com/ansible/2.9/modules/unarchive_module.html)
- [copy](https://docs.ansible.com/ansible/2.9/modules/copy_module.html)
- [template](https://docs.ansible.com/ansible/2.9/modules/template_module.html)
- 
-----------------------
- [ignore_errors](https://docs.ansible.com/ansible/latest/user_guide/playbooks_error_handling.html)
## Role playbook 
This is just an example of how to use the role.
```
---
- name: "Installing LAMP in centos"
  hosts: servers
  become: true
  roles:
    - lamp
```
