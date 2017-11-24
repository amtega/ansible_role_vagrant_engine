# vagrant_engine

This is an [Ansible](http://www.ansible.com) role to setup vagrant engine.

## Requirements

- Ansible >= 2.0

## Role Variables

Here is a list of all the default variables for this role, which are also available in `defaults/main.yml`.

```yaml
---
# Role default lower priority variables

# List of users to add to vagrant group. This is usefull to allow concrete users
# to manage vagrant without being root

vagrant_engine_users: []

```

## Dependencies

None.

## Example Playbook

This is an example playbook:

```yaml
---

- hosts: all
  roles:
    - vagrant_engine
```

## Testing

```shell
$ cd vagrant_engine/test
$ ansible-playbook main.yml --become
```

## License

Not defined.

## Author Information

- Daniel Sánchez Fábregas ([daniel.sanchez.fabregas@xunta.gal](mailto:daniel.sanchez.fabregas@xunta.gal)). Amtega - Xunta de Galicia
