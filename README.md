Debian common
=============

A debian specicific init. tasks

Requirements
------------

Debian based host

Role Variables
--------------

- `apt_cache_days` - perform apt's cache update if its older than this number of days (default: 1)
- `apt_update` - perform apt's cache update only if set (default: False)

- `sys_locales` - list of locales to generate: `pl_PL.UTF-8` by default
- `sys_packages` - list of packages to install


Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: debian_common, apt_update: yes }

License
-------

BSD
