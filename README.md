## cron-apt

[![CI](https://github.com/Oefenweb/ansible-cron-apt/workflows/CI/badge.svg)](https://github.com/Oefenweb/ansible-cron-apt/actions?query=workflow%3ACI)
[![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-cron--apt-blue.svg)](https://galaxy.ansible.com/Oefenweb/cron_apt)

Set up cron-apt in Debian-like systems.

#### Requirements

None

#### Variables

* `cron_apt_mailto`: [default: `root`]: The email address to send mail to
* `cron_apt_mailon`: [default: `upgrade`]: When to send email about the cron-apt results
* `cron_apt_options`: [optional]: General apt options that will be passed to all `APTCOMMAND` calls
* `cron_apt_syslogon`: [optional]: When to send the cron-apt results to syslog (e.g. `upgrade`, `changes`)

## Dependencies

None

#### Example

```yaml
---
- hosts: all
  roles:
    - cron-apt
```

#### License

MIT

#### Author Information

Mischa ter Smitten

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-cron-apt/issues)!
