Role Name
=========

This Ansible role for installs and configurs Apache2 on Ubuntu. The role ensures that Apache2 and related packages are installed, the service is started and enabled, and, if the default site is enabled, makes a smoke test on the default Apache site.

Requirements
------------

- Ansible 2.9 or later.
- SSH access to the target systems.
- Sudo privileges on the target systems for the executing user.

Role Variables
--------------

The only variable needed to run this role is defined during the execution of the role task itself.

Dependencies
------------

None.

Example Playbook
----------------

    - name: Apache2 installation and configuration 
      hosts: web-server
      become: true
      roles: 
      - role: apache_role

License
-------

MIT

Author Information
------------------

This role was created in April of 2024.