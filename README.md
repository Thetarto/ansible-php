# Ansible PHP
[![CI](https://github.com/supertarto/ansible-php/workflows/CI/badge.svg?event=push)](https://github.com/supertarto/ansible-php/actions?query=workflow%3ACI)

Install and configure PHP with Ansible.

## Requirements

None

## Tested plateforms
* Debian 10 (Buster)

## Role Variables
List of packages instaled by the role. It's not yet possible to install php from source.
```yaml
php_packages:
  - php7.3
```
Name of the webserver daemon used by PHP. For example, apache2, httpd, nginx... Needed.
```yaml
php_webserver_daemon: "apache2"
```

* Optional variables:
** php_apache_configuration
** php_cli_configuration:
Used with key/value like:
```yml
php_apache_configuration:
- name: opcache.memory_consumption
  value: 256
```
## Examples
```yml
---
- hosts: somehost
  roles:
    - supertarto.php
```

## Installation
```
ansible-galaxy install supertarto.php
```
## License
GPL V3.0
