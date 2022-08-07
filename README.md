Proxmox: Dark Theme
===================

An ansible role that (un)installs the PVE Discord Dark theme.

Requirements
------------

N/A

Role Variables
--------------

| Variable  | Default |                     Description                      |
| :-------: | :-----: | :--------------------------------------------------: |
| `install` | `true`  | Specifies whether to install or uninstall the theme. |

Dependencies
------------

N/A

Example Playbook
----------------

To install the theme, simply include the role:

``` yml
---
- hosts: pve
  remote_user: root

  roles:
    - role: proxmox-dark-theme
```

To uninstall the theme, specify `install: false` as a variable:

``` yml
---
- hosts: pve
  remote_user: root

  roles:
    - role: proxmox-dark-theme
      vars:
        install: false
```

License
-------

MIT

Author Information
------------------

A role developed by [Mircea-Pavel ANTON](https://www.mirceanton.com).
