# Ansible Example

Brief explaination of each major component

## Playbook

The playbook `playbook.yml` defines roles and tasks that should be run.

## Role

The `hello` role defines a list of tasks can can be run. These roles can be
shared between multiple playbooks instead of duplicating lists of tasks in
those playbooks.

## Inventory

The inventory file defines the groups of hosts that we would run our playbooks
on. With the format:

```
[groupname:vars]
ansible_user=<ssh-username>

[groupname]
url
url
...
```

The `groupname` would then be used in the `hosts` section of the playbooks.
