Virtualbox
==========
An ansible role to install VirtualBox.

The role adds the VirtualBox repository, installs the VirtualBox software and rebuilds the kernel with the needed driver. Vagrant is also installed by default. Blank `virtualbox_vagrant_url` to avoid installing Vagrant.

Requirements
------------
See `meta/main.yml`.

Role Defaults
--------------
See `defaults/main.yml`.

Dependencies
------------
Make sure EPEL is available, ie using role `geerlingguy.repo-epel`. It is needed to install some packages needed for rebuilding VirtualBox drivers, ie `dkms`.

Example Playbook
----------------
Example:
```
- hosts: servers
  roles:
    - geerlingguy.repo-epel
    - virtualbox
```

TODO
----
None.

License
-------

BSD

Author Information
------------------
Robin Bruckenstein-Kowitz (robin@rockefeller.edu)
Luis Gracia while at [EMBL-EBI](http://www.ebi.ac.uk/):
- luis.gracia [at] ebi.ac.uk
- GitHub at [luisico](https://github.com/luisico)
- Galaxy at [luisico](https://galaxy.ansible.com/luisico)
