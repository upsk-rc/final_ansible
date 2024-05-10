php_role
=========

This Ansible role is designed to automate the process of installing PHP and related packages on a Linux system. It ensures that PHP, PHP modules, and configuration files are set up correctly. Additionally, if the Apache2 default site is enabled, it performs a smoke test to verify the installation.

Requirements
------------

- Ansible 2.9 or later.
- SSH access to the target systems.
- Sudo privileges on the target systems for the executing user.
- Apache2 installed.

Role Variables
--------------

The following variable is used in this role:
default_file: This variable contains the path to a local php info file that is copied to the target host.

Dependencies
------------

None.

Example Playbook
----------------

- name: PHP installation and configuration 
  hosts: web-server
  become: true
  roles: 
    - role: php_role

License
-------

This project is licensed under the MIT License.

Author Information
------------------

This role was created in April of 2024.