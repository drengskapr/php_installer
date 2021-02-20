PHP Installer
=========

Installs desired version of `php` along with some popular additional packages. Uses [deb.sury.org](https://deb.sury.org/) repository.

Requirements
------------

Debian 10

Role Variables
--------------

`php_version` -- desired `php` version to install.

Example Playbook
----------------
```
- name: Server installation according to roles
  hosts: all
  remote_user: root
  roles:
    - role: php_installer
      vars:
        php_version: 7.4
```

License
-------

BSD
