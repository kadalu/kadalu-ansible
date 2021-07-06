Role Name
=========

This role prepares everything needed for setting up kadalu with native gluster quota.

Requirements
------------

This role uses ansible k8s module which requires:
- python >=2.7
- openshift >= 0.6
- PyYAML >= 3.11

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

gluster_quota_user ---> User on the gluster nodes that can call gluster's cli
# Location where we store the private keys on the kube master nodes
privatekey_location ---> Path on the kubernetes nodes where we store the private ssh key

ssh_key_name ---> key name which is existing locally, if you change it - add it to the gitignore


Dependencies
------------

---

Author Information
------------------

Strahil Nikolov
