Role Name
=========

With this script you can send an archive of mediafiles and a database backup. They will be unarchived and placed in the right place, and the database will be restored to the point of backup.

Requirements
------------

Created docker containers according to my project, i.e.:
- container with django project named web, 
- container with database named db, 
- nginx container named nginx.

Role Variables
--------------

You must indicate the path to the backups and change the name of the user who uses this script in main_playbook.yml file.

Example Playbook
----------------

~~~bash 
ansible-playbook -i hosts.yaml main_playbook.yml --ask-become-pass 
~~~

License
-------

BSD

