An opinionated Ansible collection to provision Linux servers and workstations with my dotfiles, packages, and Jinja-templated configs. Idempotent, reproducible, and tuned for my workflow. Use it to replicate my environment or as a starting point.

Next workable version is on [ansible-linux](https://github.com/greykaizen/ansible-linux)

Requirements: Ansible 2.9+, Git, and sudo on target hosts. Primary playbook: site.yml.

Quick start: git clone https://github.com/greykaizen/super-ansible.git && cd super-ansible
Local run: ansible-playbook -i inventory/localhost.ini site.yml --connection=local --become
Remote run: ansible-playbook -i inventory/hosts site.yml --become -u <user>

Customize by editing inventory, group_vars/ and host_vars/ or changing role defaults in roles/*/defaults/main.yml. Review tasks before running on production.
