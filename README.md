ansible-pip
=========
[![Build Status](https://travis-ci.org/openstax/ansible-pip.svg?branch=master)](https://travis-ci.org/openstax/ansible-pip)

Installs the appropriate version of pip and other pip packages.

Requirements
------------

N/A

Role Variables
--------------
| Name                   | Default Value | Description                                              |
| ---------------------- | ------------- | -------------------------------------------------------- |
| `pip_package`          | python-pip    | sets the python-pip package. Use python3-pip for python3 |
| `pip_version`          | 9.0.1         | sets the version of pip that should be installed         |
| `pip_install_packages` | []            | sets other pip packages to install                       |


Dependencies
------------

N/A

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      vars:
        pip_package: python3-pip
        pip_version: 9.0.1
      roles:
        - role: ansible-pip

License
-------

AGPLv3

Development & Testing
---------------------

This project uses [Molecule](http://molecule.readthedocs.io/) to aid in the
development and testing; the role is unit tested using
[Testinfra](http://testinfra.readthedocs.io/) and
[pytest](http://docs.pytest.org/).

To develop or test you'll need to have installed the following:

* Linux (e.g. [Ubuntu](http://www.ubuntu.com/))
* [Docker](https://www.docker.com/)
* [Python](https://www.python.org/) (including python-pip)
* [Ansible](https://www.ansible.com/)
* [Molecule](http://molecule.readthedocs.io/)
