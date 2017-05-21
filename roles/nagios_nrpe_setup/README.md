Role Name
=========

Install EPEL respository.
Install Nagios client (nrpe) packages and plugins.
Deploys nrpe.cfg from template.
Starts and enables nrpe.

Requirements
------------

Nagios server

Role Variables
--------------

defaults/main.yml contains EPEL repository variables (can leave default) and nrpe allowed_hosts variable (meant to be overridden).

Dependencies
------------

none

Example Playbook
----------------

    ---
    - name: Configure nrpe
      hosts: "{{ host_group }}"
      roles:
        - nagios_nrpe_setup


License
-------

GPLv2


Author Information
------------------

Douglas Jones, RHCA

Red Hat, Inc.

douglas@redhat.com
