[![](https://img.shields.io/travis/com/ckaserer/ansible-role-keymap/master?style=flat-square)](https://travis-ci.com/ckaserer/ansible-role-keymap)
![gplv3](https://img.shields.io/badge/license-GPL%20v3.0-brightgreen.svg?style=flat-square)
![Maintenance](https://img.shields.io/maintenance/yes/2021?style=flat-square)

# ckaserer.keymap

```
ansible-galaxy install ckaserer.keymap
```

---

## Set the keymap

Alternativly you can set `hosts` to a group of ansible nodes or `all`.

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
