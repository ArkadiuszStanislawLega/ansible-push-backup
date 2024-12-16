Ansible push backup
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

Other links
------------

1. Automatic server installation: <https://github.com/ArkadiuszStanislawLega/ansible-start-server>
2. Creating a backup: <https://github.com/ArkadiuszStanislawLega/ansible-make-backup>
3. Serwer docker compose: <https://github.com/ArkadiuszStanislawLega/docker-django-web-server>


License
-------

BSD

