copy_backup_to_host
=========

Copies the archive from ./files/{{ backup_filename }} to the host, then unpacks the archive.

Requirements
------------

You should place the backup archive in the ./files/filename directory, where filename is the name of the variable in ./vars/main.yml file.

Role Variables
--------------

You need to change the backup_filename variable in the ./vars/main.yml file to the name of the backup archive file.


License
-------

BSD

