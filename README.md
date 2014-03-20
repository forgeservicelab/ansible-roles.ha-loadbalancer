ha-loadbalancer
===============

Sets up a cluster of two load balancers for High Availability, managed by heartbeat.

Requirements
------------

All pre-requisites are specified on the roles this builds upon. ha-loadbalancer has no pre-conditions of its own.

Role Variables
--------------

- `OS_FLOATIP` - The public IP through which this load balancing cluster will be exposed to the world.
- `heartbeat_service_name` - The name of the load balancing server as it appears on `/etc/init.d`. Defaults to haproxy.

Dependencies
------------

This role depends on:

- The [load-balancer role](https://git.forgeservicelab.fi/ansible-roles/load-balancer)
- The [heartbeat role](https://git.forgeservicelab.fi/ansible-roles/heartbeat)

Author Information
------------------

[Forge Servicelab Team](http://forgeservicelab.fi)
