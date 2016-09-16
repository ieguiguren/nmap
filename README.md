Nmap     
====

Downloads from Nmap's SVN and compiles nmap. Also downloads and install geolocation from maxmind for scripts like ip-geolocation-maxmind.

Requirements
------------

For now, this script only works on "Debian-like" distros.

Role Variables
--------------

No variables defined. The role will install nmap in the /usr/local/{bin. lib, share} with SSL and LUA support.

Dependencies
------------

No dependencies. This role installs everything it should need.

Example Playbook
----------------

    - hosts: all
      roles:
         - ieguiguren.nmap

License
-------

BSD

Author Information
------------------

Any fix request or suggestions or merge-request will be gladly attended via http://github.com/ieguiguren/nmap

