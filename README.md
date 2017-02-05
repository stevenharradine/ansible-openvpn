# ansible-openvpn
[Ansible](http://www.ansible.com/) role to install openvpn from source with TLS1.2 enabled

[![Licence](https://img.shields.io/badge/Licence-ISC-blue.svg)](https://opensource.org/licenses/ISC)
[![Role](https://img.shields.io/ansible/role/6168.svg)](https://galaxy.ansible.com/detail#/role/6168)
[![Platforms](http://img.shields.io/badge/platforms-ubuntu-lightgrey.svg)](#)

Tunables
--------
* `openvpn_server_port` (integer) - port to listen on
* `openvpn_server_key_size` (integer) - rsa key size to be used
* `openvpn_server_compile_from_source` (boolean) - should we compile and build openvpn from source?  If no you will install from the outdated repo that does not support TLS1.2
* `openvpn_server_firewall_enabled` (boolean) - use UFW to harden this installation?  Only disable if you know what your doing and have a firewall upstream.
* `openvpn_server_firewall_allow_ssh` (boolean) - allow ssh connections to this box?  Disabled by default, if you dont have physical access to the box and need remote connections its probally safe to enable.
* `openvpn_server_firewall_allow_dns` (boolean) - allow DNS requests through the firewall
* `openvpn_server_firewall_dns_gateway` (boolean) - your networks gateway (where the dns requests will be routed from)

Dependencies
------------
None

Example Playbook
----------------
    - hosts: servers
      roles:
         - role: stevenharradine.openvpn

License
-------
[MIT](https://tldrlegal.com/license/mit-license)

Contributors
------------
* Steven Harradine
