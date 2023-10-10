# Ansible PHP
[![CI](https://github.com/supertarto/ansible-php/workflows/ci.yml/badge.svg?event=push)](https://github.com/supertarto/ansible-php/actions/workflows/ci.yml)

Install and configure PHP with Ansible.

## Requirements

None

## Tested plateforms
* Debian 10 (Buster)
* Debian 11 (Bullseye)
* Debian 12 (Bookworm)

## Role Variables
List of packages instaled by the role. It's not yet possible to install php from source.
```yaml
php_packages:
  - "php{{php_default_version_debian}}"
```
Name of the webserver daemon used by PHP. For example, apache2, httpd, nginx... Needed.
```yaml
php_webserver_daemon: "apache2"
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
