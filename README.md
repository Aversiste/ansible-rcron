ansible-rcron
=============

Configure rcron, a cron scheduler with redundancy and failover.

Requirements
------------

A `rcron` package. The source code is available [here](https://github.com/bpineau/rcron).

Role Variables
--------------

    rcron_cluster_name: an arbitrary name for your rcon instances.
    rcron_state: either `passive' or `active'. The later is the default.

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: all
      roles:
      - role: ansible-rcron
        rcron_cluster_name: crawlers

License
-------

ISC

Author Information
------------------

Written by Tristan Le Guern on behalf of Deveryware.
