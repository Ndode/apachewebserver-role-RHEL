Role Name
=========

apache role designed to install and setup an apache webserver on RHEL.

Requirements
------------
a control machine which has ansible installed and a remote system that needs to be managed by control machine in my case centos 7 for control machine and fedora for host.

Role Variables
--------------
main components used for this role were the tasks directory, files and handlers, with each containing its own files.Task has 3 files in main.yml- one for installing apache, another for configuring apache and the 3rd for starting apache. files contained the configurations file and downloaded image to be used in index.html file.  site.yml contains the host on which the webserver was to be run.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

playbook that is run: site.yml

    - hosts: fedora host IP
      roles:
         - apache



