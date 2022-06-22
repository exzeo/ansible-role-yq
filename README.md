Ansible Role YQ
=========

Installs yq Command Line on Debian/Ubuntu servers. 
Releases: https://github.com/mikefarah/yq/releases

Role Variables
--------------

```
# Version of 'yq' to install, defaults to latest version
yq_version: ""

# Toggling this will uninstall from the server
uninstall: false
```

Example Playbooks
----------------

Minimal:
```
- name: Install CLI
  hosts: all
  roles:
    - role: exzeo.yq
```

Specific Version:
```
- name: Install CLI
  hosts: all
  roles:
    - role: exzeo.yq
      vars:
        yq_version: "4.24.5"
```

Uninstall:
```
- name: Install CLI
  hosts: all
  roles:
    - role: exzeo.yq
      vars:
        uninstall: true
```