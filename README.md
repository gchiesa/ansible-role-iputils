Role Name
=========

This role set the facts based on the modules loaded. 

Requirements
------------

none

Role Variables
--------------

The list of role variables depends on the modules activated by the play / role 

### Common variables
```
host_natted: false # set to true if the host ip is natted 
```

### Consul
consul_bootstrap_hostname: 127.0.0.1

### Etcd
etcd_bootstrap_hostname: 127.0.0.1


Dependencies
------------
none

Example Playbook
----------------

This role is aimed to be used as dependency of other roles. Check the following meta example: 

```
    dependencies:
      - {role: gchiesa.docker}
      - {role: gchiesa.iputils, modules: ['common']}
```      

License
-------

BSD

