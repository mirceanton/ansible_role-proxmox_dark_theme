<h1>
  Since Proxmox now comes with a dark UI option by default, this repo has been archived and is now read-only!!
</h1>

Proxmox: Dark Theme
===================

An ansible role that installs the [PVE Discord Dark](https://github.com/Weilbyte/PVEDiscordDark) theme by [Weilbyte](https://github.com/Weilbyte).

Requirements
------------

N/A

Role Variables
--------------

|         Variable          |  Type  |         Default          |                      Description                       |
| :-----------------------: | :----: | :----------------------: | :----------------------------------------------------: |
| `proxmox_dark_theme_dest` | string | `/opt/PveDiscordDark.sh` | The path at which the theme installer should be saved. |

To check the default variables, take a look at the [defaults](defaults/main.yml) file.

Dependencies
------------

N/A

Example Playbook
----------------

``` yml
---
- name: Install the dark theme on all pve hosts.
  hosts: pve
  remote_user: root

  roles:
    - role: mirceanton.proxmox_dark_theme
      proxmox_dark_theme_dest: /opt/installers/dark-theme.sh
```

License
-------

MIT

Author Information
------------------

A role developed by [Mircea-Pavel ANTON](https://www.mirceanton.com).
