# Ansible Role: vector

Роль устанавливает Vector и отправляет события в ClickHouse.

## Role Variables

| Variable | Default | File |
| --- | --- | --- |
| vector_version | 0.22.1 | defaults/main.yml |
| vector_clickhouse_ip | localhost | defaults/main.yml |
| clickhouse_db_name | logs | defaults/main.yml |
| vector_url | packages.timber.io | vars/main.yml |
| vector_config_dir | /etc/vector | vars/main.yml |

## Example Playbook

- hosts: vector
  become: true
  roles:
    - vector
