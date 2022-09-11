# Ansible Role for Postgresql
![Version](https://img.shields.io/github/v/release/mach1el/ansible_postgresql?color=red&style=plastic) ![License](https://img.shields.io/github/license/mach1el/ansible_postgresql?color=orange&style=plastic)

Auto build,deploy Postgres database with ansible

## Role variables
See [`default/main.yml`](https://github.com/mach1el/ansible_postgresql/blob/master/defaults/main.yml)

## Role pathes

```
├── defaults
│   └── main.yml
├── handlers
│   └── main.yml
├── tasks
│   ├── configure.yml
│   ├── initialize.yml
│   ├── main.yml
│   └── setup_debian.yml
└── templates
├──  pg_hba.conf.j2
├── postgresql.conf.j2
└── postgres.sh.j2
```

## Example playbook
```
- name: Initialize postgresql
  hosts: all
  become: true
  roles: 
    - 'mach1el.ansible_postgresql'
```
