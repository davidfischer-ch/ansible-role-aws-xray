# Ansible Role AWS X-Ray

Library of Ansible plugins and roles for deploying various services.
See [ansible-roles](https://github.com/davidfischer-ch/ansible-roles) for additional documentation.

This repository hosts the role aws-xray and may depend of other roles and plugins of the library.

## Dependencies

See [meta](meta/main.yml).

## Variables

TODO VARIABLES

## Example

Setup the daemon.

### Playbook

```
---

- hosts:
    - web
  roles:
    - aws-xray
  vars:
    aws_xray_role_action: setup

    aws_xray_version: 3.x
    aws_xray_release_checksum: sha256:5563498bd5c6dd08556827bc87aec269f0655349fe1079caf2d21d0049fc90ca
    aws_xray_daemon_mode: supervisor

```

## License

See [LICENSE.rst](LICENSE.rst).

## Authors

See [AUTHORS](AUTHORS).

2014-2022 - David Fischer
