# Ansible role scaffold

An Ansible role scaffold with the structure I follow for my Ansible roles.

Based on the style and work of [geerlingguy](https://github.com/geerlingguy).

Tests with [Test-Kitchen](http://kitchen.ci/), [Vagrant](https://www.vagrantup.com/) and [Serverspec](http://serverspec.org).

### Vagrant

Check [Vagrant](vagrant/README.md) readme.

### Test Kitchen

Installation:

    # gem install test-kitchen kitchen-ansible kitchen-docker kitchen-vagrant

```
$ kitchen list

Instance                     Driver   Provisioner      Verifier  Transport  Last Action
default-ubuntu-precise64     Vagrant  AnsiblePlaybook  Busser    Ssh        <Not Created>
default-ubuntu-trusty64      Vagrant  AnsiblePlaybook  Busser    Ssh        <Not Created>
default-geerlingguy-centos6  Vagrant  AnsiblePlaybook  Busser    Ssh        <Not Created>
```

    $ kitchen converge ubuntu-precise64
    

    $ kitchen verify ubuntu-precise64


    $ kitchen destroy 


Check [Test Kitchen](http://kitchen.ci/) doc.

### Serverspec

Check [Serverspec](http://serverspec.org/resource_types.html) site for examples.

### License

MIT

### Author

This role was created in 2016 by Raul Martinez.
