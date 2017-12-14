wp_update
=========

 This package allows you setup the package wp-cli in the user PATH.

Requirements
------------

This package dont have extra requirements.

Role Variables
--------------

In this role there are few customizable variables:
- WP_INSTALL_DIR: This directory will contain the script wp and will be added to the path. By default ~/bin/

- PROFILE_PATH: File where is setup the user profile. by default uses ~/.profile

- FORCE_INSTALL: (boolean) When it set to true it will install de latest version in the user home.


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

Inventory file:

[webservers]
myexample.com ansible_host=1.1.1.1 PROFILE_PATH=/etc/bashrc FORCE_INSTALL=true

Playbook:

    - hosts: webservers
      roles:
         - wp_cli
