ansible-pritunl
=========

This ansible role installs the Pritunl VPN server.

Requirements
------------

Ansible 2.10.8

Role Variables
--------------

|Variable|Description|
|--------|-----------|
| mongodb_version | The version of MongoDB to install |
| distribution_release | The Ubuntu release name for MongoDB repo |

Dependencies
------------
N/A

Example of how to use the role
----------------

    - hosts: localhost
      become: true
      gather_facts: yes
      
      vars:
        mongodb_version : 3.2
        distribution_release: "focal"
    roles:
      - role: ansible-pritunl

License
-------

MIT

Author Information
------------------
[Yurii Onuk](https://onuk.org.ua)
