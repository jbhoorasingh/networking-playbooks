Role Name
=========

This role is used to set the NTP server on heterogeneous network devices. 

Requirements
------------

- arista.eos
- cisco.ios
- cisco.nxos

Role Variables
--------------

| Variable | Descriptions | #Default |
| :---: | :---: | :---: |
| ntp_server1 | This is the preferred NTP server | time.google.com |
| ntp_server2 | This is the preferred NTP server | time.windows.com |

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

    - hosts: 
         - arista
         - ios
      roles:
         - { role: ntp, ntp_server1: 1.1.1.1, ntp_server2: 1.1.1.2 }


