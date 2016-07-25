ansible-dockerpy
=========

Installs `docker-py` on Debian Jessie.

Requirements
------------

Only runs on Debian Jessie.

Role Variables
--------------

`dockerpy_version` can be set to the version of `docker-py`, which should be installed.

Dependencies
------------

No dependencies.

Example Playbook
----------------

    - hosts: servers
      roles:
         - ansible-dockerpy

License
-------

BSD
