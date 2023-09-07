Role Name
=========

This role is used to set up local authentication on a network device

Requirements
------------

- arista.eos (TBA)
- cisco.ios
- cisco.nxos (TBA)

Role Variables
--------------


|      Variable      |       Descriptions       |   #Default   |
|:------------------:|:------------------------:|:------------:|
|   account1_name    | Local account1 username  | local_admin1 |
| account1_password  | Local account1 password  |   Coolaid    |
| account1_privilege | Local account1 privilege |      15      |
|   account2_name    | Local account2 username  | local_admin2 |
| account2_password  | Local account2 password  |  Pineapple   |
| account2_privilege | Local account2 privilege |      1       |
|  enable_password   |      Enable secret       |  Watermelon  |


Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

    - hosts:
         - ios
      roles:
         - { role: local_authentication, account1_name: "local_admin1", account1_password: "Coolaid", account2_name: "local_admin2", account2_password: "Pineapple",}


