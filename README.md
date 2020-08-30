Debian-Zsh
==========

Install ZSH as default shell for local users

Requirements
------------

This role requires a debian compliant system such as ubuntu.

Role Variables
--------------

system:
  users:
    - user1
    - user2
  sudoers:
    - user2
  removed:
    - user3

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: cowops.debian-zsh, system.users: user1,user2, system.sudoers: user2 }

Tasks
-----

  - Install [ZSH](http://www.zsh.org/) shell
  - Install sudo command
  - Add system and git users
  - Remove deprecated users
  - Import system users' keys
  - Import root and git keys

License
-------

BSD
