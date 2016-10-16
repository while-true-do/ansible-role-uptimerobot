# Ansible Role: Uptimerobot
| A very simple role to pause and start uptimerobot monitors.

## Installation

Galaxy Link: <https://galaxy.ansible.com/while-true-do/uptimerobot>

```
ansible-galaxy install while-true-do.uptimerobot
```

Github Link: <https://github.com/CHANGEME>

```
git clone CHANGEME
```

## Requirements

None.

## Dependencies

None.

## Role Variables
You have to set the following variables to use this role. See [here](https://uptimerobot.com/api), how you can use it.

```
# defaults/main.yml
utr_api_key: ''
utr_monitor_id: ''
utr_monitor_state: ''
```

## Example Playbook
To pause a Monitor for WebServer1, you can do the following example:

```
- hosts: WebServer1
  roles:
    - { role: while-true-do.uptimerobot, utr_api_key: 12345-1234512345, utr_monitor_id: 12345, utr_monitor_state: paused }
    - { role: AnotherRoleThatDoesSomething }
    - { role: while-true-do.uptimerobot, utr_api_key: 12345-1234512345, utr_monitor_id: 12345, utr_monitor_state: started }
```

## License

This work is licensed under a [BSD License](https://opensource.org/licenses/BSD-3-Clause).

## Contribute / Bugs

**bug reports:** <https://github.com/while-true-do/CHANGEME/issues>

**contributers:** <https://github.com/while-true-do/CHANGEME/graphs/contributors>

## Author Information

**blog:** <https://blog.while-true-do.org>

**github:** <https://github.com/daniel-wtd>

**contact:** [mail@while-true-do.org](mailto:mail@while-true-do.org)
