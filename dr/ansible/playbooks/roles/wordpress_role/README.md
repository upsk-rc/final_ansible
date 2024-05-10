wordpress_role
=========

This Ansible role is designed to automate the process of preparing a server for a WordPress installation, as well as downloading, installing, and configuring WordPress on Linux systems. The role takes care of preparing the necessary directories, disabling the Apache2 default site, and installing and enabling the WordPress site.

Requirements
------------

- Ansible 2.9 or later.
- SSH access to the target systems.
- Sudo privileges on the target systems for the executing user.
- Apache2 insatlled.
- PHP installed.

Role Variables
--------------

- wp_host: wordpress site name and domain (e.g. dpr.example.com).
- mysql_root_password: mysql password for the root user.
- mysql_db: name of the wordpress mysql database.
- mysql_user: user for the wordpress mysql database.
- mysql_user_password: mysql password for the mysql_user user.

Dependencies
------------

Depends on apache_role and php_role.

Example Playbook
----------------

- name: Wordpress installation and configuration
  hosts: web-server
  vars: 
    mysql_db_host: example.host
    mysql_db: example.database
  roles: 
    - role: wordpress_role

License
-------

This project is licensed under the MIT License.

Author Information
------------------

Role created in April of 2024.
