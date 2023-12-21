Setup User
=========

The role is used to define and create a new user on remote server, setup it's password SSH loging key, disables SSH root login and login without user name and prompt.

Requirements
------------

This role is specifically developed for Ubuntu-based systems. While it may work on other Debian-based distributions, it has not been tested on them.


Role Variables
--------------

The role uses variables which can be found in `defaults/main.yml`. You can override these variables in your playbook if necessary.

Dependencies
------------

No other Ansible roles are required for this role.

Example Playbook
----------------

``yaml
---
- name: Setup New User
  hosts: all
  become: yes
  roles:
    - setup_user
```
