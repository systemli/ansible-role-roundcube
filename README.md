# ansible-role-roundcube

[![Build Status](https://github.com/systemli/ansible-role-roundcube/workflows/Molecule/badge.svg?branch=master)](https://github.com/systemli/ansible-role-roundcube/actions?query=workflow%3AIntegration)

Install and configure Roundcube.
This includes configuration of the Roundcube Getmail Plugin.
You can choose a custom skin `larry-custom` that has additional links to accout settings.

## Dependencies

You need to install a web and database server before using this role.
Also, you need to configure the webserver to to deliver vhost `{{ roundcube_domain }}`.

## Role Variables

see `defaults/main.yml`

## Download

Download latest release with `ansible-galaxy`

$ ansible-galaxy install systemli.roundcube

## Example Playbook

```
- hosts: servers
  roles:
    - { role: systemli.roundcube }
```

## License

GPL

## Author Information

https://www.systemli.org
