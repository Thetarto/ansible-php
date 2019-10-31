# Ansible-php
[![Build Status](https://travis-ci.org/supertarto/ansible-php.svg?branch=master)](https://travis-ci.org/supertarto/ansible-php)

Install and configure PHP with Ansible.

## Requirements

None

## Tested plateforms
* Debian 9 (Stretch)
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
## Examples
## Installation
## License
GPL V3.0
