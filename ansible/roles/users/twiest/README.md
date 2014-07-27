Role Name
========

Adds the twiest user

Requirements
------------

None

Role Variables
--------------

mtk_users: Contains all user account info
mtk_users.twiest.uid: The uid for the twiest user
mtk_users.twiest.gid: The gid for the twiest group
mtk_users.twiest.groups: a comma separated list of groups to which the twiest user should belong
mtk_users.twiest.authorized_keys: An array of public keys to add to twiest's authorized_keys file
mtk_users.twiest.email: e-mail address for the twiest user


Dependencies
------------

None

Example Playbook
-------------------------

    - hosts: servers
      roles:
         - { role: users/twiest, mtk_users: { twiest: { uid: 1000, gid: 1000, groups: 'wheel,audio', authorized_keys: ['key1','key2'], email: user@mail.org } } }

License
-------

MIT

Author Information
------------------

Thomas Wiest
