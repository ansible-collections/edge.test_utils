
# Ansible Edge Working Group Test Utilities

[![GitHub Super-Linter](https://github.com/ansible-community/edge.test_utils/workflows/Lint%20Code%20Base/badge.svg)](https://github.com/marketplace/actions/super-linter)[![Codecov](https://img.shields.io/codecov/c/github/-cop/infra.osbuild)](https://codecov.io/gh/ansible-collections/edge.test_utils)

[Ansible Collection](https://docs.ansible.com/ansible/latest/user_guide/collections_using.html)
with various [roles](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_reuse_roles.html),
[playbooks](https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_intro.html), scripts, and 
miscellaneous helper utilities in service of testing the content created by the
[Ansible Edge Automation Working Group](https://github.com/ansible/community/wiki/Edge-Automation).

## Installing

To install this collection and its dependencies, you will need to use the [Ansible](https://github.com/ansible/ansible) `ansible-galaxy` command:

```shell
ansible-galaxy collection install git+https://github.com/ansible-collections/edge.test_utils
```

## How to use

You will need a RHEL, Centos Stream, or Fedora system that you can connect to
remotely via `ssh`, and a playbook to call the desired roles to result in the
desired functionality. Each role has it's own documentation specific to its
provided automation.

To use the example playbooks provided in this repository, please create an
inventory file that only has the osbuild build server(s) listed in them as these
example playbooks use the `all` Ansible [group](https://docs.ansible.com/ansible/latest/inventory_guide/intro_inventory.html#inventory-basics-formats-hosts-and-groups)
as the [host patten](https://docs.ansible.com/ansible/latest/inventory_guide/intro_patterns.html).

