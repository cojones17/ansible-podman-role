Role Name
=========

This Ansible role deploys a simple Hello, World Docker application by leveraging both Ansible and Podman. This role can be run from any laptop or server that has a supported version of Ansible installed. 

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

```
- name: ansible podman play
  hosts: adm
  remote_user: student
  become: yes
  become_method: sudo 
  roles:
    - { role: ansible-podman-role } 
```

Roadmap
-------
- Enhance usage of variables to make the role more container image agnostic 

License
-------

BSD

Author Information
------------------
This role was created in 2022 by [Connor Jones](https://github.com/cojones17/) and [Patrick Freeman](https://github.com/freemanpdwork)
