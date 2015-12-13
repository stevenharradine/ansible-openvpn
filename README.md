# ansible-autodeploy

Simple deployment tool with hooks 

[![Platforms](http://img.shields.io/badge/platforms-ubuntu-lightgrey.svg?style=flat)](#)

TODO: install from source for TLS1.2 support

wget https://swupdate.openvpn.org/community/releases/openvpn-2.3.8.tar.xz

tar -xf openvpn-2.3.8.tar.xz

cd openvpn-2.3.8/

sudo apt-get install libssl-dev liblzo2-dev libpam0g-dev

./configure

Tunables
--------
* `hostname` (string) - The hostname to set on the server

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
