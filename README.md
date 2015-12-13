# ansible-openvpn
[Ansible](http://www.ansible.com/) role to install openvpn from source with TLS1.2 enabled

[![Licence](https://img.shields.io/badge/Licence-ISC-blue.svg)](https://opensource.org/licenses/ISC)
[![Role](https://img.shields.io/ansible/role/6393.svg)](https://galaxy.ansible.com/detail#/role/6269)
[![Platforms](http://img.shields.io/badge/platforms-ubuntu-lightgrey.svg)](#)

Tunables
--------
* `openvpn_port` (integer) - port to listen on
* `openvpn_key_size` (integer) - rsa key size to be used
* `openvpn_compile_from_source` (boolean) - should we compile and build openvpn from source or use?  If no you will install from the outdated repo that does not support TLS1.2

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
