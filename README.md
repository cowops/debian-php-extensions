Debian-PHP-Extensions
=====================

Useful PHP extensions

Requirements
------------

This role requires a debian compliant system such as ubuntu.

Role Variables
--------------

debian:
    version: wheezy
php:
    version: '55'
    extensions:
        - php5-curl
        - php5-dbg
        - php5-intl
        - php5-mcrypt
        - php5-mysqlnd
        - php5-apcu
        - php5-geoip
        - php5-imagick
        - php5-memcache
        - php5-mongo
        - php5-readline
        - php5-redis

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: cowops.debian-php-extensions, debian.version: wheezy, php.version: '55', php.extensions: php5-curl,php5-mcrypt }

Tasks
-----



License
-------

BSD
