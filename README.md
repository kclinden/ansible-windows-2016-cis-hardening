Ansible Windows 2016 CIS Hardening
=========

This Ansible Role will configure a Windows Server 2016 system to be compliant with the CIS Microsoft Windows Server 2016 RTM (Release 1607) Benchmark v1.2.0.

Requirements
------------

This Ansible Role will require that the Windows Collection be installed and available.

Role Variables
--------------

Ansible variables are listed below, along with default values in the `defaults/main.yml`

| Variable              | Default | Description                                     |
|-----------------------|---------|-------------------------------------------------|
| run_account_policies  | true    | Used to turn on or off the account policy tasks |
| is_domain_controller  | false   | Used to turn on DC Only tasks                   |
| disable_admin_account | false   | Used to turn on the disable admin account task  |

Dependencies
------------

- Windows Collection

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      roles:
         - ansible-windows-2016-cis-hardening

License
-------

Apache 2.0

Author Information
-------
Kasey Linden
kclinden.github.io
