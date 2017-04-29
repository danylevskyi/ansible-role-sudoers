# Ansible Role: Sudoers

Add specified users to passwordless sudo group.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    sudoers_users: []

A list of users who will be added to passwordless sudo group.

## Dependencies

None.

## Example Playbook

    - hosts: servers

      vars:
        sudoers_users:
          - example_user

      roles:
         - { role: danylevskyi.sudoers }

## License

BSD / MIT

## Author Information

This role was created in 2017 by [Dmytro Danylevskyi](http://dmytro.danylevskyi.com/).
