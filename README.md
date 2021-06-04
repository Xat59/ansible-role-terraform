# terraform

[![Build Status](https://api.travis-ci.com/Xat59/ansible-role-terraform.svg)](https://travis-ci.com/github/Xat59/ansible-role-terraform) ![Apache 2.0 Licence](https://img.shields.io/hexpm/l/plug.svg) ![Ansible](https://img.shields.io/badge/ansible-2.10.x-green.svg)

Ansible role that installs [`tfswitch` tool](https://tfswitch.warrensbox.com) in order to get multiple versions of Hashicorp [`terraform`](https://www.terraform.io) binary installed.
Plus, you can choose to install [`terragrunt` wrapper](https://terragrunt.gruntwork.io/) from [`tgswitch`](https://github.com/warrensbox/tgswitch).

## Prerequisites

- ![ansible](https://img.shields.io/badge/ansible-2.10.x-green.svg)

## Installation

```yaml
- hosts: servers
  roles:
    - role: xat.terraform
      tfswitch_user: xat
      terraform_versions:
        - latest
        - 0.14
        - 0.13
      install_terragrunt: true
```

## Usage

Once installed, you can use `tfswitch -b ~/.local/bin/terraform` to install or switch between terraform versions.

If you choose to `install_terragrunt`, then use `tgswitch -b ~/.local/bin/terragrunt` to install or switch between terragrunt versions.

## Versioning

For the versions available, see the [tags on this repository](https://github.com/Xat59/ansible-role-terraform/tags).

Additionaly you can see what change in each version in the [CHANGELOG.md](CHANGELOG.md) file.

## Authors

- **xat** - [xat](https://github.com/Xat59)
