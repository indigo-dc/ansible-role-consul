Role Name
=========

Install consul agent in agent or server mode (depending on the variable `consul_mode`) and dnsmaq setting . 
This role has been specifically developed to be used for the deployment of Mesos in the framework of INDIGO-DataCloud project.

Role Variables
--------------

- `docker_bridge_ip` 
- ``

Dependencies
------------

- `ansible-role-docker`

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

Apache Licence v2 [1]

[1] http://www.apache.org/licenses/LICENSE-2.0


