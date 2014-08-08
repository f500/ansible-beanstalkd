Beanstalkd
========

Install and start beanstalkd

Requirements
------------

Debian Wheezy with the package python-pycurl and python-software-properties installed.

Role Variables
--------------

    beanstalkd_listen_addr: 0.0.0.0
    beanstalkd_listen_port: 11300
    beanstalkd_enabled: "yes"

Example Playbook
-------------------------

    - hosts: servers
      roles:
         - { role: f500.beanstalkd }

License
-------

LGPL

Author Information
------------------

Jasper N. Brouwer, jasper@nerdsweide.nl

Ramon de la Fuente, ramon@delafuente.nl
