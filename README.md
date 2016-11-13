Nginx uwsgi proxy
=================


Nginx proxy for uwsgi container

Role Variables
--------------

- `domains` - list of domains (required)
- `http_port` - default: 80
- `ssl` - provide SSL connection channel (default: False)
- `http_redirect` - if both above variable and this is set - provide :80->https redirect
- `cert` - public SSL certificate path 
- `cert_key` - private SSL certificate path

Dependencies
------------

- xkoralsky.nginx_base

Example Playbook
----------------

    - hosts: servers
      roles:
        - { role: nginx_uwsgi_proxy, domains: [ example.com ] }

License
-------

BSD
