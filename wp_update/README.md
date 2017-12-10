wp_update
=========

 This package allows you to install and upgrade your wordpress instance

Requirements
------------

You need install wp-cli before run this role.

Role Variables
--------------

In this role there are few customizable variables:
- BACKUP_DIRECTORY: This variable allows to setup the directory where backups will be stored.

- WORDPRESS_HOME: The root of the wordpress installation.

- LOGFILE: This file will store the result of the command execution.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

Inventory file:

[webservers]
myexample.com ansible_host=1.1.1.1 WORDPRESS_HOME=/var/www/myblog/

Playbook:

    - hosts: webservers
      roles:
         - wp_update
