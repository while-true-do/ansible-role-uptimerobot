[![Build Status](https://travis-ci.org/while-true-do/ansible-role-uptimerobot.svg?branch=master)](https://travis-ci.org/while-true-do/ansible-role-uptimerobot)

# Ansible Role: Uptimerobot
| A very simple role to pause and start Uptimerobot monitors.

## Motivation

[Uptimerobot](https://uptimerobot.com/) is a free monitoring tool with an integrated status-page and lots of monitor capabilities. Pausing and Starting the monitors during ansible runs is a key feature of maintenance windows to avoid unwanted alerts.

## Installation

Install from [Ansible Galaxy](https://galaxy.ansible.com/while-true-do/uptimerobot)

```
ansible-galaxy install while-true-do.uptimerobot
```

Install from [GitHhub](https://github.com/while-true-do/ansible-role-uptimerobot)

```
git clone https://github.com/while-true-do/ansible-role-uptimerobot.git while-true-do.uptimerobot
```

## Requirements

Valid Uptimerobot Account and [API Key](https://uptimerobot.com/api).

Used Modules:

-   [uptimerobot](http://docs.ansible.com/ansible/latest/uptimerobot_module.html)


## Dependencies

None.

## Role Variables
You have to set the following variables to use this role.

```
# defaults/main.yml

wtd_utr_api_key: ''
wtd_utr_monitor_id: []
wtd_utr_monitor_state: ''
# You can set this to false, if you are using pre_task/post_task in your play.
wtd_utr_flush_handlers: 'true'
```

## Testing

All tests are located in [test directory](./tests/).

Basic testing:

```
bash ./tests/test-spelling.sh
bash ./tests/test-ansible.sh
```

## Contribute / Bugs

Thank you so much for considering to contribute. Every contribution helps us.
We are really happy, when somebody is joining the hard work. Please have a look
at the links first.

-   [Contribution Guidelines](./docs/CONTRIBUTING.md)
-   [Create an issue or Request](https://github.com/while-true-do/ansible-role-uptimerobot/issues)
-   [See who was contributing already](https://github.com/while-true-do/ansible-role-uptimerobot/graphs/contributors)

## License

This work is licensed under a [BSD License](https://opensource.org/licenses/BSD-3-Clause).

## Author Information

Blog: [blog.while-true-do.org](https://blog.while-true-do.org)

Mail: [hello@while-true-do.org](mailto:hello@while-true-do.org)

