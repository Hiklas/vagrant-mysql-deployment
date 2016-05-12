## Overview

Intended as an environment to play with MySQL 

## Quickstart

* Install ansible
* Run vagrant up
* Run vagrant ssh to connect and play with the VM 

## Setup

### Pre-requisites

* VirtualBox
* Vagrant
* Python 

The code was developed and tested on a Mac but should work fine on other platforms that meet the above requirements.


### Installing ansible

Since Ansible has been packaged for use with pip I've used virtualenv for python to allow a local installation that doesn't need admin access or muck up any of your system libraries.  I prefer this approach as it's cleaner and has less in the way of side-affects.  Feel free to install ansible from RPMs/.deb or other package managers onto your system natively if that is easier for you.

Create a virtual python environment and activate it

```
virtualenv ansible-env
. ansible-env/bin/activate
```

Install ansible

```
pip install ansible
```

### Inital VM

Start VM using this

```
vagrant up
```

## Background

### Ansible MySQL module

There is a specific module for Ansible that allows certain configuration tasks to be carried out.  More information on the [module](http://docs.ansible.com/ansible/mysql_user_module.html).

