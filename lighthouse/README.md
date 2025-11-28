# Ansible Role: Lighthouse

## Описание

Развертывание lighthouse

## Требования

- Rocky Linux 8/9
- Ansible 2.1+

## Переменные

```yaml
lighthouse_repo: "https://github.com/VKCOM/lighthouse.git"
lighthouse_dest: "/opt/lighthouse"
nginx_port: 80
```

## Использование

```yaml
- hosts: web_servers
  roles:
    - lighthouse
```

## Пример

```yaml
- hosts: monitoring
  vars:
    nginx_port: 8080
  roles:
    - lighthouse
```

## Лицензия

MIT
