# Ansible Role: Wordpress

Clone Wordpress and configure the db.

## Requirements

Tested CentOS 7

## Role Variables

Available variables are listed below, along with default values `defaults/main.yml`

```yml
wordpress_directory: /var/wordpress
wordpress_user: vagrant
wordpress_version: 4.7.4
wordpress_servername: wordpress.local

wordpress_settings_configuration:
  - regexp: "database_name_here"
    line: "define('DB_NAME', 'wordpressdb');"
  - regexp: "'username_here"
    line: "define('DB_USER', 'root');"
  - regexp: "password_here"
    line: "define('DB_PASSWORD', 'MYSQL_ROOT_PASSWORD');"
```

## Dependencies

None

# License

MIT

# Author Information

Apostolos Tovletoglou [ansible-role-wordpress](https://github.com/tovletoglou/ansible-role-wordpress)
