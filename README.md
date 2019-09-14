ansible_nginx
=========

Role is intended to install and configure NGINX on a Red Hat system.

Requirements
------------

_Optional:_ Run it with sudo password prompt:
```
ansible-playbook --ask-become-pass main.yml -l remote
BECOME password: 
```

Role Variables
--------------

No variables.

Dependencies
------------

If it is a new system, it may require [`ansible_epel`](https://github.com/110marc/ansible_epel) role to be played prior `ansible_nginx`

Example Playbook
----------------

An example of how to use your role:

    - hosts: servers
      become: yes
      roles:
         - ansible_epel *optional
         - ansible_create_user

License
-------

BSD

Author Information
------------------

> https://github.com/110marc
