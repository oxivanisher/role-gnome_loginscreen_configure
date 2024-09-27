gnome_loginscreen_configure
===========================

This role configures the Gnome login screen.

Role Variables
--------------

| Name                                         | Comment                              | Default value |
|----------------------------------------------|--------------------------------------|---------------|
| gnome_loginscreen_configure_background_image | The user on the system for which the mounts are configured  |           |
| gnome_loginscreen_configure_hidden_users     | The CIFS username on the nas |          |
| gnome_loginscreen_configure_disable_userlist | The CIFS password on the nas |          |
| gnome_loginscreen_configure_banner_message   | A list of dicts containing `src` and `dest`. | `[]`     |

Example Playbook
----------------
```yaml
- name: Configure WOL
  hosts: clients
  roles:
    - role: oxivanisher.linux_desktop.wol
```

License
-------

BSD

Author Information
------------------

This role is part of the [oxivanisher.linux_desktop](https://galaxy.ansible.com/ui/repo/published/oxivanisher/linux_desktop/) collection, and the source for that is located on [github](https://github.com/oxivanisher/collection-linux_desktop).
