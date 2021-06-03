# terraform

![Build Status](https://api.travis-ci.com/Xat59/ansible-role-terraform.svg) ![Apache 2.0 Licence](https://img.shields.io/hexpm/l/plug.svg) ![Ansible](https://img.shields.io/badge/ansible-2.10.x-green.svg)

Ansible role that installs [`tfswitch` tool](https://tfswitch.warrensbox.com) in order to get multiple versions of Hashicorp `terraform` binary installed.

## Prerequisites

- ![ansible](https://img.shields.io/badge/ansible-2.10.x-green.svg)

## Usage

```yaml
- hosts: servers
  roles:
    - role: xat.terraform
      tfswitch_user: xat
```

## Versioning

For the versions available, see the [tags on this repository](https://github.com/Xat59/ansible-role-terraform/tags).

Additionaly you can see what change in each version in the [CHANGELOG.md](CHANGELOG.md) file.

## Authors

- **xat** - [xat](https://github.com/Xat59)
