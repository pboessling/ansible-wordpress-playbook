# ansible-wordpress-playbook

Ansible playbook to setup WordPress together with nginx, PHP-FPM, and MariaDB, PHP-FPM.

## Requirements

- CentOS/RHEL 7.4
- Ansible 2.4
- Vagrant 2.0.1+
- VirtualBox 5.1.30+

## License

[Creative Commons Attribution 3.0 Unported License.](LICENSE)

## Author Information

Created by [Philippe Bößling](https://www.gihub.com/pboessling).

Based on: https://github.com/ansible/ansible-examples/tree/master/wordpress-nginx_rhel7

## TODO
- rename default.conf to wordpress.conf -> will be renamed to actual domain name later
- provide default.conf for http and https which returns a 403
- https://github.com/savoirfairelinux/ansible-nginx/blob/master/tasks/htpasswd.yml