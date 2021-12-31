# Ansible role: systemd-networkd
Management of network interfaces, systemd style

## Requirements
Debian bullseye

## Role Variables
+ `networkd_extra`: dict of (path, contents) pairs for
  files to add under `/etc/systemd/network/`
+ `networkd_eth0_naming` (default: false): boolean, whether to
  disable predictable network interface naming
+ `ifup_disable` (default: true): whether to disable `networking.service`
  and let systemd-networkd manage interfaces rather than `ifup`
  (`/etc/networking/`)

## Playbooks
+ `main.yml`: apply role
+ `uninstall.yml`: remove. Run before removing config from inventory.

## Dependencies
+ [ho-ansible.systemd](https://github.com/ho-ansible/systemd)

## License
+ Ansible role licensed [MIT](LICENSE)

## Author Information
+ Ansible role by [Sean Ho](https://github.com/ho-ansible/)
