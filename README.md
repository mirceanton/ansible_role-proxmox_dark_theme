Proxmox: Dark Theme
===================

An ansible role that installs the [PVE Discord Dark](https://github.com/Weilbyte/PVEDiscordDark) theme by [Weilbyte](https://github.com/Weilbyte).

Requirements
------------

N/A

Role Variables
--------------

|          Variable          |  Type  |         Default          |                      Description                       |
| :------------------------: | :----: | :----------------------: | :----------------------------------------------------: |
| `proxmox_dark_theme_shell` | string |          `bash`          |     The shell to use when launching the installer.     |
| `proxmox_dark_theme_dest`  | string | `/opt/PveDiscordDark.sh` | The path at which the theme installer should be saved. |

To check the default variables, take a look at the [defaults](defaults/main.yml) file.

Dependencies
------------

N/A

Example Playbook
----------------

``` yml
---
- hosts: pve
  remote_user: root

  roles:
    - role: mirceanton.proxmox_dark_theme
```

License
-------

MIT

Author Information
------------------

A role developed by [Mircea-Pavel ANTON](https://www.mirceanton.com).
