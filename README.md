# Sudoers

Sudoers is an Ansible role to add users to an Ubuntu installation, each with passwordless sudo capabilies and SSH login.

# Variables:

## sudoers_group
`sudoers_group: "wheel"`
 
The group to place new users in.

## sudoers_users

```
sudoers_users:
  - name: "hephaestus"
    key: "keys/hephaestus.pub"
```

The list users to add, each with passwordless sudo capabilities and SSH login. Each user must have a `name` and `key` specified.