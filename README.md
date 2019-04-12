egeneralov.timescaledb
======================

Provide timescaledb installation.

Requirements
------------

Debian-based system, supported by official postgresql repository.

Note: supported postgresql versions:
  - 9.6
  - 10
  - 11

Role Variables
--------------

See `defaults/main.yml` for full list. Also see [egeneralov.postgresql](https://github.com/egeneralov/postgresql).

Dependencies
------------

- [egeneralov.postgresql](https://github.com/egeneralov/postgresql).

Example Playbook
----------------

    ---
    - hosts: timescaledb
      vars:
        pgdg_users:
          - user: zabbix
            password: zabbix
            database: zabbix
      remote_user: root
      roles:
        - egeneralov.timescaledb

License
-------

MIT

Author Information
------------------

Eduard Generalov <eduard@generalov.net>
