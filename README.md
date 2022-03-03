# ansible-role-kind

![Ansible](https://github.com/avnes/ansible-role-kind/actions/workflows/ansible.yaml/badge.svg)

Ansible role for installing kind.

## Requirements

Poetry. Install it from <https://python-poetry.org/docs/>

## Role Variables

```yaml
kind_version: 3.7.2
kind_for_all_users: true # If false it will install in in the users ~/bin directory
command_shell: bash         # Must be bash or zsh
```

## Dependencies

None

## Example Playbook

```yaml
- hosts: all
  roles:
     - { role: avnes.kind }
```

## For pip compability

```bash
poetry export --dev --output requirements.txt
```

## Test

```bash
poetry install
poetry shell
molecule test
```

## License

MIT

## Author Information

<https://github.com/avnes>
