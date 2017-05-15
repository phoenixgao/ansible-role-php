# Ansible Role PHP

## Variables
```yml
# Whether to use a custom apt repository, default to false, could be "ppa:ondrej/php"
php_apt_repository: false
# PHP version, default to 7.0
php_version: 7.0
```

## Extensions
This role will install these php extensions:
```yml
- "php{{ php_version }}-fpm"

- "php{{ php_version }}-curl"
- "php{{ php_version }}-gd"
- "php{{ php_version }}-json"
- "php{{ php_version }}-mbstring"
- "php{{ php_version }}-mcrypt"
- "php{{ php_version }}-mysql"
- "php{{ php_version }}-opcache"
- "php{{ php_version }}-xml"
- "php{{ php_version }}-zip"
```