![Ansible Lint](https://github.com/johanneskastl/ansible-role-opensuse_configure_transactional_update_service/workflows/Ansible%20Lint/badge.svg)

opensuse_configure_transactional_update_service
=========

Configure the transactional-update.service on openSUSE

Requirements
------------

None.

Role Variables
--------------

- `transactional_updates_reboot_method` (String): reboot method that is to be
  used with the transactional-update.service

Check the
[manpage](https://manpages.opensuse.org/Tumbleweed/transactional-update/transactional-update.conf.5.en.html) for details.

Dependencies
------------

None

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
    - role: 'johanneskastl.opensuse_configure_transactional_update_service'
      transactional_updates_reboot_method: kured
```

License
-------

BSD-3-Clause

Author Information
------------------

I am Johannes Kastl, reachable via kastl@b1-systems.de.
