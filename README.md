role_app_nfs
=========

Sets up a NFS server.


TODO
------------

Instead of disabling firewalld, the necessary firewallports should be opened for NFS.


Requirements
------------

playbook_baseinstall

Role Variables
--------------

Expects a variable "role_app_nfs_exports" that defines the necessary exports:
``` 
role_app_nfs_exports:
   /export/secondary: "*(rw,async,no_root_squash,no_subtree_check)"
   /export/primary: "*(rw,async,no_root_squash,no_subtree_check)"
```

Dependencies
------------

Nothing to say here.

Example Playbook
----------------

Used in playbook_acs_single_node.

License
-------

GNU Public License v3.0

Author Information
------------------

Melanie Desaive, m.desaive@mailbox.org
