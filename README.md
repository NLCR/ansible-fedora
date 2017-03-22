Fedora 4
=========

Simple role to install Fedora 4.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

fedora_url: https://github.com/fcrepo4/fcrepo4/releases/download/fcrepo-4.7.1/fcrepo-webapp-4.7.1-jetty-console.jar
fedora_version: 4.7.1
fedora_checksum: md5:a086463b317423000111f7dbc45fb674
fedora_path: /opt/{{ fedora_url | basename }}

Dependencies
------------

- NLCR.java-oracle

defaults/main.yml
java_oracle_url: http://download.oracle.com/otn-pub/java/jdk/8u121-b13/e9e7ea248e2c4826b92b3f075a80e441/jre-8u121-linux-x64.rpm

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: NLCR.fedora, url: fedora_url: https://github.com/fcrepo4/fcrepo4/releases/download/fcrepo-4.7.1/fcrepo-webapp-4.7.1-jetty-console.jar, fedora_version: 4.7.1, fedora_checksum: md5:a086463b317423000111f7dbc45fb674 }

License
-------

BSD

Author Information
------------------

Rudolf Kreibich
