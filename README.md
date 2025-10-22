# super-ansible
Space for the ansible configs.

Next workable version is on [ansible-linux](https://github.com/greykaizen/ansible-linux)

To know the name of the distro ansible is using
> ansible localhost -m setup -a 'filter=ansible_distribution'

- structure
```
  ansible-local/
    ├── roles/
    │   ├── flatpak/
    │   │   ├── tasks/
    │   │   │   └── main.yml
    │   │   └── vars/
    │   │       └── packages.yml
    │   ├── ubuntu/
    │   │   ├── tasks/
    │   │   │   ├── main.yml
    │   │   │   └── packages.yml
    │   │   └── vars/
    │   │       └── packages.yml
    │   ├── arch/
    │   │   ├── tasks/
    │   │   │   ├── main.yml
    │   │   │   ├── packages.yml
    │   │   │   └── aur.yml
    │   │   └── vars/
    │   │       ├── packages.yml
    │   │       └── aur.yml
    │   └── fedora/
        ├── tasks/
        │   ├── main.yml
        │   └── packages.yml
        └── vars/
            └── packages.yml
```

- workables command for local testing
> ansible-playbook local.yml

