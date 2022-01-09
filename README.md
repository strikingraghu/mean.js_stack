Role Name
=========

This role installs and configure the system with MEAN.JS stack components.
At this moment, this role is developed for CentOS/RHEL platforms and will be working towards updating playbook for other OS platforms as well.
Currently, this role installs below components:
```
-- rubygems
-- gcc-c++
-- make
-- git
-- fontconfig
-- bzip2
-- libpng-devel
-- ruby
-- ruby-devel
-- sass
-- mongodb
-- nodejs
-- bower
-- gulp
```

Requirements
------------

Ensure internet connectivity is available to download YUM packages to the system that is going to run MEAN.JS stack

Role Variables
--------------

We haven't used much for roles, will be enhancing in later point in time

Dependencies
------------

We don't see a need for an additional dependencies mentioned in the role

Example Playbook
----------------

Below is the example to call this role via main.yml file:

```
---
- hosts: all
  gather_facts: true
  become: true

  tasks:
    - include_role:
        name: mean-stack
```

License
-------

MIT/BSD

Author Information
------------------

This role was created in Jan 2022 by Raghavendra Guttur from Bangalore, India
