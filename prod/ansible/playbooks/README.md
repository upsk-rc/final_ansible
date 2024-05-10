# Ansible Project

The Ansible Project automates the deployment of configurations for two identical unconnected environments using Ansible. It manages various components, including web servers, databases, and Windows servers.

Notes: 
This repository was created as the final project for the Automation module in a SysAdmin course and is intended solely for academic purposes.
The contents of this README file were made with the help of Copilot.

## Project Structure

- inventory/: Includes inventory files for different environments (e.g., production, disaster recovery);
- roles/: Holds reusable Ansible roles for configuring web servers, databases, etc.;
- apache_wordpress_playbook.yml: playbook that uses the different roles configured in the roles/ directory;
- update_playbook.yml: independent playbook that updates operating systems; 
- find_environment_playbook.yml: playbook used by other playbooks to determine in which environment the ansible playbook being executed.

## Introduction

This project aims at automating the deployment of configurations for two identical unconnected environments using Ansible and is composed of:

- Disaster Recovery Environment
    - Control Node for Ansible
    - Webserver, with Apache2, PHP and Wordpress;
    - DBserver, with MySQL;
    - Windows Server, with MySQL Workbench

- Production Environment
    - Control Node for Ansible
    - Webserver, with Apache2, PHP and Wordpress;
    - DBserver, with MySQL;
    - Windows Server, with MySQL Workbench 

## License

This project is licensed under the [MIT License](LICENSE).