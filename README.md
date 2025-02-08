gnome_loginscreen_configure
===========================
[![Ansible Lint](https://github.com/oxivanisher/role-gnome_loginscreen_configure/actions/workflows/ansible-lint.yml/badge.svg)](https://github.com/oxivanisher/role-gnome_loginscreen_configure/actions/workflows/ansible-lint.yml)

This role configures the Gnome login screen.

Role Variables
--------------

| Name                                         | Comment                              | Default value |
|----------------------------------------------|--------------------------------------|---------------|
| gnome_loginscreen_configure_background_image | A file set as gnome login background. It needs to be in the `{{ playbook_dir }}/files/gnome_loginscreen_configure/` directory  |           |
| gnome_loginscreen_configure_hidden_users     | Users which are hidden from the login screen | `[]`        |
| gnome_loginscreen_configure_disable_userlist | Should the user list be disabled at the login screen |  `false`       |
| gnome_loginscreen_configure_banner_message   | A custom banner message for the login screen | ``     |

Example Playbook
----------------
```yaml
- name: Configure Gnome login screen
  hosts: clients
  roles:
    - role: oxivanisher.linux_desktop.gnome_loginscreen_configure
```

License
-------

BSD

Author Information
------------------

This role is part of the [oxivanisher.linux_desktop](https://galaxy.ansible.com/ui/repo/published/oxivanisher/linux_desktop/) collection, and the source for that is located on [github](https://github.com/oxivanisher/collection-linux_desktop).
