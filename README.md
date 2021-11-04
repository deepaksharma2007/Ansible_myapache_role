ansible_myapache_role
=========

myapache role is used to configure apache webserver using httpd product. 

Requirements
------------

Ansible must be configured well in your controller node
We must have connectivity between controller node and Managed node. You can check by command (ansible webservers -m ping) .
Also make host name of servers in inventory file must be "webservers". Add all servers under "webservers" host to configure apache webservers.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. I used basically two variable
1. pkgs: This is used to tell which software will be install.
2. rule: This is used to create firewall rule . So we can access http and https services.


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: webservers
      roles:
         - { role: path }
      
      here path = where you download "myapache" role

License
-------

BSD

Author Information
------------------
The author of this roley Deepak Sharma.
