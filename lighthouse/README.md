# Ansible Role: Lighthouse

## Описание

Развертывание lighthouse

## Требования

- Rocky Linux 9
- Ansible 2.1+

## Переменные

```yaml
nginx_port: 80
lighthouse_dest: "/opt/lighthouse"
```

## Использование

```yaml
- name: "Deploy Lighthouse"
  hosts: lighthouse
  become: true
  roles:
    - lighthouse
```
