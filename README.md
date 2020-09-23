[![](https://img.shields.io/travis/com/ckaserer/ansible-role-keymap/master?style=flat-square)](https://travis-ci.com/ckaserer/ansible-role-keymap)
![gplv3](https://img.shields.io/badge/license-GPL%20v3.0-brightgreen.svg?style=flat-square)
![Maintenance](https://img.shields.io/maintenance/yes/2021?style=flat-square)

# ckaserer.keymap

Set the keymap of your choice on your linux systems with the `ckaserer.keymap` ansible role.

First you need to install the role on the node from which you will execute ansible via

```
ansible-galaxy install ckaserer.keymap
```

---

## Set the keymap

```
- hosts: localhost
  tasks:
    - name: "Include ckaserer.keymap"
      include_role:
        name: "ckaserer.keymap"
        apply:
          become: true
        vars:
          keymap: de
```

Alternativly you can set `hosts` to a group of ansible nodes or `all`.
