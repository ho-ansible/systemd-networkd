# Ansible Role: systemd-networkd
Management of network interfaces, systemd style

## Requirements
Debian stable

## Role Variables
None

## Handlers
+ `update initramfs`: regenerates the ram disk used by the kernel
  to find the root filesystem during boot

## Dependencies
+ [ho-ansible.systemd](https://github.com/ho-ansible/systemd)

## License
MIT

## Author Information
Sean Ho, https://github.com/ho-ansible/
