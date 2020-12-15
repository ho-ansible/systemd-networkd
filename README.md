# Ansible role: systemd-networkd
Management of network interfaces, systemd style

## Requirements
Debian stable

## Role Variables
None

## Handlers
+ `update initramfs`: regenerates the ram disk used by the kernel
  to find the root filesystem during boot

## Playbooks
+ `main.yml`: apply role
+ `uninstall.yml`: remove. Run before removing config from inventory.

## Dependencies
+ [ho-ansible.systemd](https://github.com/ho-ansible/systemd)

## License
+ Ansible role licensed [MIT](LICENSE)

## Author Information
+ Ansible role by [Sean Ho](https://github.com/ho-ansible/)
