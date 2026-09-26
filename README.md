# My Fedora 

My custom ansible roles combined in one playbook for initial Desktop Fedora (Gnome) config, which fits my needs.

Currently supported Fedora version: **44 (Gnome)**

---

Things these roles do:
- change gnome icons, cursor
- configures gnome settings via dconf
- installs several gnome extensions
- `/etc/ssh_config`
- VSCode installation and `.json` config
- flatpak remote and installs several flatpaks
- syncthing installation
- git config in my home directory
- installs several rmp packages with dnf and deletes defaults that I don't need
- sets hostname
- sets global umask
- updates whole system

---

Requirements:
- ansible

---

`myfedora44.yaml` combines all roles and tasks. To run it use this command:
```bash
ansible-playbook myfedora44.yaml --ask-become-pass
```