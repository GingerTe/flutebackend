Flute backend
=========

[![Ansible Galaxy](https://img.shields.io/badge/galaxy-gingerte.flutebackend-blue.svg)](https://galaxy.ansible.com/gingerte/flutebackend/)

Requirements
------------

Java 8

Role Variables
--------------

* flute_build: flute build number
* flute_user: user for flute service user
* flute_group: the group for flute service user (default valute is flute)
* flute_java_memory: memory for flute service
* flute_dir: where to intall flute (default value is /opt/flute)
* java_home: where java home located
* flute_log_dir directory for logs output (default is /var/log/flute)
* flute_user  user for flute service (default is flute3)


Example Playbook
----------------

    - hosts: servers
      vars:
         java_packages:
          - openjdk-8-jre
        java_home: /usr/lib/jvm/java-8-openjdk-amd64
      roles:
        - role: geerlingguy.java
        - role: gingerte.fluteansible

License
-------

MIT

Author Information
------------------

https://corchestra.ru/en
