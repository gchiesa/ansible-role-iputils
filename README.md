gchiesa.iputils
===============

This is a role containing utilities used as requirement from the other roles

Requirements
------------

none

Role Variables
--------------

The modules can be activated by passing the variable:
```
modules = ["common", ...]
```

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

