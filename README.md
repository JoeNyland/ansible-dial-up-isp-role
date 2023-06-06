# Ansible Dial-ISP Role
=======================

[![CI](https://github.com/JoeNyland/ansible-dial-up-isp-role/actions/workflows/ci.yml/badge.svg)](https://github.com/JoeNyland/ansible-dial-up-isp-role/actions/workflows/ci.yml)

This role configures a host to simulate a dial-up ISP.

Requirements
------------

The following physical items are required:

* A host to act as the dial-up ISP server. I've tested this on a Raspberry Pi 4B and a Raspberry Pi Zero.
* A serial modem connected to the host which will act as the ISP side. I have tested with a USRobotics Courier 'V.Everything' modem.
* A Linksys/Cisco VoIP ATA. I have tested with a PAP2T, but this should work with other ATAs.

Role Variables
--------------

See [`defaults/meta.yml`](./defaults/main.yml).

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: server
  roles:
    - role: joenyland.dial_up_isp
```

License
-------

MIT

Author Information
------------------

⌨️ with ❤️ by [Joe Nyland](https://joe.nyland.io)
