# Ansible Role: Remarkable Templates and Splashscreen

[![CI](https://github.com/JakobLichterfeld/ansible-role-remarkable_templates_and_splashscreen/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/JakobLichterfeld/ansible-role-remarkable_templates_and_splashscreen/actions/workflows/ci.yml)
[![Publish role on Ansible Galaxy](https://github.com/JakobLichterfeld/ansible-role-remarkable_templates_and_splashscreen/actions/workflows/publish_role_on_ansible_galaxy.yml/badge.svg?branch=main)](https://github.com/JakobLichterfeld/ansible-role-remarkable_templates_and_splashscreen/actions/workflows/publish_role_on_ansible_galaxy.yml)

Change Remarkable Splash Screen and import own templates.

- Backup Splash Screen
- Copy own Splash Screen to device
- Copy Templates and templates.json to device
- Restart the Remarkable interface to ensure changes are applied

Since Remarkable Tablets do not support Python, this role utilizes low-level Ansible functions. That is why this role is not idempotent.

## Requirements

None.

## Role Variables

None.

## Dependencies

None.

## Example Playbook

```yaml
---
- hosts: remarkable
  gather_facts: false
  become: false

  roles:
    - role: jakoblichterfeld.remarkable_templates_and_splashscreen

```

## License

MIT

## Author Information

This role was created in 2023 by [Jakob Lichterfeld](https://github.com/JakobLichterfeld).
