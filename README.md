esxi_install
=========
 
This is a role created for installing an ESXI operative system in a Lenovo xcc managed server.
 
Requirements
------------
 
* Ansible
* xcc managed server.
* community.general
 
Role Variables
--------------
  
### defaults/main.yml
Default nginx installation variables.
 
* username: Username credential to login into xcc.
* password: Password credential to login into xcc.
* baseuri: Redfish API URL.
 
### vars/main.yml

* bootdevice: Name of the booting device in which the ISO is mounted.
 
Dependencies
------------
 
---
 
Example Playbook
----------------
 
   - hosts: localhost
     become: true
     roles:
       - role: xcc_install
         username: "My_user"
         password: "My_passwd"
         base_uri: "[ip:port]"
       
 
License
-------
 
-
 
Author Information
------------------
 
Oviedo Matias
Schinca Mauro