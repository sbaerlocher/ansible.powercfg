# Ansible Role: powercfg

[![Build Status](https://travis-ci.org/sbaerlocher/ansible.powercfg.svg?branch=master)](https://travis-ci.org/sbaerlocher/ansible.powercfg) [![license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://sbaerlo.ch/licence) [![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-powercfg-blue.svg)](https://galaxy.ansible.com/sbaerlocher/powercfg)

## Description

Disable and re-enable hibernation on a computer that is running Windows

## Installation

```bash
ansible-galaxy install sbaerlocher.powercfg
```

## Requirements

None

## Role Variables

| Variable                     | Default | Comments (type) |
| :--------------------------- | :------ | :-------------- |
| powercfg_hibernation_disable | false   |                 |
| powercfg_standby_ac_disable  | true    |                 |
| powercfg_standby_ac_time     | 20      |                 |

## Dependencies

None

## Example Playbook

```yml
- hosts: all
  roles:
    - sbaerlocher.powercfg
```

## Changelog

### 1.2.0

- Compatible with 2.9.0

### 1.1.0

- add Support for standby disable

### 1.0.0

- initial commit

## Author

- [Simon Bärlocher](https://sbaerlocher.ch)

## License

This project is under the MIT License. See the [LICENSE](https://sbaerlo.ch/licence) file for the full license text.

## Copyright

(c) 2018, Simon Bärlocher
