# Ansible Role for Postgresql
![License](https://img.shields.io/github/license/mach1el/ansible-role-postgresql?color=orange&style=plastic)

Auto build,deploy Postgres database with ansible

## Role variables
See [`default/main.yml`](https://github.com/mach1el/ansible-role-postgresql/blob/master/defaults/main.yml)

## Role pathes

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

## Example playbook
  
	---
	- name: Building kamailio for local server
		hosts: local_server
		become: true
		
		roles: - '../ansible-role-kamailio'
