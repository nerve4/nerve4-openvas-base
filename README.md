# openVAS - base

An Ansible role that install OpenVAS to Rocky8. More info about openVAS: [link](https://www.openvas.org/)


## Requirements

Make sure, you made your vars file with valid path to custom template or you can use Default vars.

You need `ansible 2.13.7` to run this module

The Role also use `community.general collection` and `ansible.posix collection` modules. To install it, use: `ansible-galaxy collection install community.general` / `ansible-galaxy collection install ansible.posix`. 


## Tasks descriptionsa

- main.yml - Run the OS check and run the relevant playbook
- rhel-install-openvas-base.yml - Deploy openVAS on Rhel


## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```
- hosts: servergroup
  become: true
  become_user: lee

  vars_files:
    - vars/main.yml
    
  roles:
    - nerve4-openvas-base
```

## Maintainer Information
Lee | 2023