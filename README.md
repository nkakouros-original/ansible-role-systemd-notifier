[![Galaxy](https://img.shields.io/badge/galaxy-nkakouros.systemd_notifier-blue.svg)](https://galaxy.ansible.com/nkakouros/systemd_notifier/)

ansible-role-systemd-notifier
=========

Installs a notifier to inform the user of failures of systemd services

Description
-----------

The role will install a script that provides the option to get email or Slack
notifications of failures of selected SystemD services. The services are
reconfigured to use the script when they stop execution abnormaly.

Requirements
------------

For Slack messages, you need to setup a hook for the role to use.

Dependencies
------------

None

Role Variables
--------------

Look at the [defaults/main.yml](defaults/main.yml) file for this roles variables and their
documentation.

Example Playbook
----------------

This is a minimal playbook:

```yaml
- hosts: server
  roles:
    - nkakouros.systemd-notifier
```

For a full example see the [molecule/default/](molecule/default/) folder.

License
-------

GPLv3

Author Information
------------------

Nikolaos Kakouros (nkak@kth.se)
