Role Name
=========

An ansible role to install add the VirtualBox repository, install the VirtualBoxsoftware and rebuild the kernel with the needed driver

Requirements
------------
All required packages are included in the tasks/main.yml file.

Role Defaults
--------------

The location of the URL needed to install the repository is listed in the defauls/main.yml file

Dependencies
------------

Make sure EPEL is available, ie using role `geerlingguy.repo-epel`. It is needed to install some packages needed for rebuilding VirtualBox drivers, ie `dkms`.

Example Playbook
----------------

    - hosts: servers
      roles:
         - virtualbox

License
-------

BSD

Author Information
------------------

Robin Bruckenstein-Kowitz (robin@rockefeller.edu)
Luis Gracia  (lgracia@rockefeller.edu)
The Rockefeller University
