Debian-Zsh
==========

Install ZSH shell

Requirements
------------

This role requires a debian compliant system such as ubuntu

Role Variables
--------------

Dependencies
------------

- cowops.debian_users role

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: cowops.debian-zsh }

Tasks
-----

  - Install [ZSH](http://www.zsh.org/) shell
  - Enable zsh for root

License
-------

BSD
