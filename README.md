Ansible Debian Bootstrap
=========

Setups a debian machine with sane defaults.

Requirements
------------

The initial machine should have a running ssh server with root login via password enabled.

Role Variables
--------------
| Variable       | Required | Comments                                                    |
| -------------- | -------- | ----------------------------------------------------------- |
| user           | yes      | Default username                                            |
| user_password  | yes      | Default user password                                       |
| id_ed25519_pub | yes      | Public ssh key which can be used to login as a default user |


Example Playbook
----------------
```yaml
- hosts: servers
  roles:
    - { role: debian-bootstrap, become: true }
```
License
-------

BSD
