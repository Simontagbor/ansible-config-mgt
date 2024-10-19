Nginx Proxy Server Role
=========

This role installs and configures Nginx as a reverse proxy server.

Requirements
------------

This role is designed for ubuntu 20+ servers.

Role Variables
--------------

The role variables include the following: 

- `nginx_proxy_server_name`: The name of the server.
- `Subnet`: The subnet of the server.
- `domain_name`: The domain name of the server.

Dependencies
------------

This role is currently dependent on the `nginx` package.

Example Playbook
----------------
  
```yaml
- hosts: servers
  roles:
    - role: nginx
      nginx_proxy_server_name: "<nginx.example.com>"
      Subnet: "<subnet>"


License
-------

BSD

Author Information
------------------

Simon Gabriel Tagbor