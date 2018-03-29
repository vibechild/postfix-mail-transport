Postfix Mail Transport Role
=========

A generic mail transport configuration using postfix

Requirements
------------

This role is intended to be included in a project with the specific variables and config files provided. This repository is the generic configuration which will be the same regardless of the specific configuration of the instances.  In other words the requirement of this repository is that it be used as a requirement in another repository.

Role Variables
--------------

software:
  - postfix
  - firewalld
  - telnet
  - mailx
  
configfiles:
  - README.md
databasefiles:
  - README.md

rootalias: you@example.com


Dependencies
------------

This role does not require any other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: postfix-mail-transport, rootalias: "you@example.com" }


Author Information
------------------

* **Devin** - *Initial work* - [Other Projects](https://github.com/vibechild)
