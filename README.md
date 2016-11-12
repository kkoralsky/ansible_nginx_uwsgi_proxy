Nginx uwsgi proxy
=================


Nginx proxy for uwsgi container

Role Variables
--------------

- `domains` - list of domains (required)
- `port` - default: 80
- `ssl` - provide SSL connection channel (default: False)
- `http_redirect` - if both above variable and this is set - provide :80->https redirect
- `cert` - public SSL certificate path 
- `cert_key` - private SSL certificate path

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
        - { role: nginx_uwsgi_proxy, domains: [ example.com ] }

License
-------

BSD
