Role Name
========

Adds the twiest user

Requirements
------------

None

Role Variables
--------------

mtk_twiest_uid: The uid for the twiest user
mtk_twiest_gid: The gid for the twiest group
mtk_twiest_groups: a comma separated list of groups to which the twiest user should belong
mtk_twiest_authorized_keys: An array of public keys to add to twiest's authorized_keys file


Dependencies
------------

None

Example Playbook
-------------------------

    - hosts: servers
      roles:
         - { role: users/twiest, mtk_twiest_uid: 1000, mtk_twiest_gid: 1000, mtk_twiest_groups: wheel,audio, mtk_twiest_authorized_keys: ['key1','key2'] }

License
-------

MIT

Author Information
------------------

Thomas Wiest
