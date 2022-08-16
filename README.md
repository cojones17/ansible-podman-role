Role Name
=========

This Ansible role deploys a simple Hello, World application by leveraging both Docker and Podman. The role can be run from any laptop or server that has Ansible installed 

Requirements
------------
- Ansible version 2.13.1+
- sshpass (optional, required if you're using a password, not certifcates to authenicate)

Role Variables
--------------
None

Dependencies
------------
None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```
- name: ansible podman play
  hosts: adm
  remote_user: student
  become: yes
  become_method: sudo 
  roles:
    - { role: ansible-podman-role } 
```

License
-------

BSD

Author Information
------------------
Connor Jones 
