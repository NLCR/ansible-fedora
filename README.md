Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

fedora_url: https://github.com/fcrepo4/fcrepo4/releases/download/fcrepo-4.7.1/fcrepo-webapp-4.7.1-jetty-console.jar
fedora_version: 4.7.1
fedora_checksum: md5:a086463b317423000111f7dbc45fb674
fedora_jar: /opt/{{ fedora_url | basename }}

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
