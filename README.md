# ansible-role-grafana

Ansible role for installing Grafana

## Variables

### General

- `grafana_hostname` [required]
- `grafana_security_admin_password` [required]
- `grafana_server_root_url` [default: `https://{{ grafana_hostname }}`]
- `grafana_traefik_router_rule` [default: `Host(``{{ grafana_hostname }}``)`]

### Docker

- `grafana_docker_image` [default: `grafana/grafana:9.4.7`]
- `grafana_image_renderer_docker_image` [default: `grafana/grafana-image-renderer:3.6.4`]
