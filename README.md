Debian-Zsh
==========

Install ZSH as default shell for local users

Requirements
------------

This role requires a debian compliant system such as ubuntu.

Role Variables
--------------

system_users:
  - user1
  - user2
system_sudoers:
  - user2

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: loranger.debian-zsh, system_users: user1,user2, system_sudoers: user2 }

Tasks
-----

  - Install [ZSH](http://www.zsh.org/) shell
  - Install sudo command
  - Add system and git users
  - Import system users' keys
  - Import root and git keys

License
-------

BSD