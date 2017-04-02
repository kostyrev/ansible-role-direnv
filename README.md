# direnv

[![Build Status](https://travis-ci.org/kostyrev/ansible-role-direnv.svg?branch=master)](https://travis-ci.org/kostyrev/ansible-role-direnv)

Installs direnv

Requirements
------------

None

Role Variables
--------------

See [defaults/main.yml](defaults/main.yml) for a list and description of
variables used in this role.

Example Playbook
----------------

```yaml
---
- hosts: all
  roles:
    - role: kostyrev.direnv
      direnv_validate_certs: "{{ false if ansible_virtualization_type == 'docker' else true }}"
```

Install From Github
-------------------

```
git clone https://github.com/kostyrev/ansible-role-direnv.git kostyrev.direnv
cd kostyrev.direnv && make install
```

License
-------

BSD

Author Information
------------------

Aleksandr Kostyrev
