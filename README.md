Role Name
=========

Ansible role to install Terraform on Linux x64 machines.

Role Variables
--------------
Here are the role variables and their default values.

    terraform_version: "0.11.3"
    terraform_dir: "/opt/terraform"

Example Playbook
----------------
requirements.yml

```
- name: ansible-role-tf
  src: https://github.com/Ambisafe/ansible-role-tf.git
```

playbook.yml

```
- name: testing role ansible-role-tf
  hosts: localhost
  gather_facts: false
  vars:
    terraform_version: "0.11.3"
    terraform_dir: "/opt/terraform"
  roles:
       - { role: ansible-role-tf }
```

Author Information
------------------
Artem Yushkov

DevOps@Ambisafe

