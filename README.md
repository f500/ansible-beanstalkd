Beanstalkd
========

Install and start beanstalkd

Requirements
------------

Debian Wheezy.

Warning: This role will install **build-essential** if it isn't already present.
Some people consider this a security risk.  If you're one of them,  you should 
remove build-essential in a role that runs later, or manually.


Role Variables
--------------

    beanstalkd_version: "1.10"
    beanstalkd_listen_addr: "0.0.0.0"
    beanstalkd_listen_port: "11300"
    beanstalkd_user: "beanstalkd"
    beanstalkd_enabled: "yes"
    
    beanstalkd_persistent: Yes
    beanstalkd_storage: "/var/lib/beanstalkd"

Warning: Changing beanstalkd_storage after an initial install will result in the
original binlog data being orphaned in the original location.

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
