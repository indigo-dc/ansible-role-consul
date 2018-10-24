consul
=========

Run consul in agent or server mode (depending on the variable `consul_mode`) in container using the image `progrium/consul` and configures consul as primary DNS for the host node and docker containers.

This role has been specifically developed to be used for the deployment of Mesos in the framework of INDIGO-DataCloud project.

Role Variables
--------------

- `docker_bridge_ip`: IP to be statically assigned to docker bridge
- `consul_servers_list`: (optional) list of consul *server* nodes - alternatively, you can use a proper inventory file specifying the hosts group [consul_servers]
- `consul_image` (default: progrium/consul)
- `consul_version` (default: latest)

Dependencies
------------

- `indigo-dc.docker`

Example Playbook
----------------

    - hosts: agents
      roles:
         - { role: indigo-dc.consul, consul_mode: "agent", consul_servers_list: ["172.10.10.1", "172.10.10.2", "172.10.10.3" ] }

License
-------

Apache Licence v2 [1]

[1] http://www.apache.org/licenses/LICENSE-2.0


