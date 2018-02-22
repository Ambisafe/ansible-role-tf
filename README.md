Installing Terraform
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
- name: terraform-cli
  src: https://github.com/Ambisafe/ansible-role-tf-cli.git
```

playbook.yml

```
- name: testing role terraform-cli
  hosts: localhost
  gather_facts: false
  vars:
    terraform_version: "0.11.3"
    terraform_dir: "/opt/terraform"
  roles:
       - role: terraform-cli
```

Author Information
------------------
Artem Yushkov

DevOps@Ambisafe

