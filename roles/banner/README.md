Role Name
=========

This role is used to set the banner on network devices. 

Requirements
------------

- arista.eos
- cisco.ios
- cisco.nxos

Role Variables
--------------

| Variable | Descriptions | #Default |
| :---: | :---: | :---: |
| banner_text | Banner text that will be displayed | #############################################\nAThis is a private system maintained by the\nCompany_Name\nUnauthorized use of this system can result in\ncivil and criminal penalties!\n############################################# |


Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

    - hosts: 
         - arista
         - ios
      roles:
         - { role: banner, banner_text: "#################\nBanner Test \nBanner Test Line2\n#################\n" }


