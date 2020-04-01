install_basic_packages
======================

This ansible roles installs the basic software packages on newly created host/s for the administration tasks.
It performs the complete update after the basic packages installation and reboots the server.

Requirements
------------

      - ansible 2.7.7

Role Variables
--------------

This role has only one variable defined in the defaults/main.yml, that is a list of packages to install on the systems

    - packages 

Dependencies
------------

None

Example Playbook
----------------

You can create a playbook with the following content to use this role :

    - hosts: servers
      roles:
         - { role: install_basic_packages }
   
For the direct one line command installation on localhost use :

	ansible-playbook --connection=local --inventory 127.0.0.1, install_basic_packages.yaml


Author Information
------------------

      Raman Deep
      1st April 2020
      deep.raman85@gmail.com

