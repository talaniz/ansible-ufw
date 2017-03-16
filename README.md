Ansible UFW
=========

[![Build Status](https://travis-ci.org/talaniz/ansible-ufw.svg?branch=master)](https://travis-ci.org/talaniz/ansible-ufw)

A simple role to manage the Ubuntu UFW for my blog project.

Requirements
------------

Ansible version 16+ as the ufw module is used.

Variables
---------

Variables can be defined in either a vars directory or the playbook directly.
`access_ports` - ports to open. Defaults to 22, 80 and 443.
`ssh_port` - port for ssh, currently used to apply rate limit.

Example Playbook
----------------

    - hosts: servers
      # Uncomment this section to use vars directly in the playbook.
      # vars:
      #    access_ports:
      #           - 80
      #           - 443
      roles:
         - talaniz.ansible-ufw

License
-------

BSD

Author Information
------------------
E-mail: antonio.alaniz@gmail.com
Website: www.antonioalaniz.com
