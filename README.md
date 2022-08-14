## Ansible ad-hoc commands

> ansible [pattern] -m [module] -a "[module options]"

- [pattern] = targeting hosts and groups
  - "all" = default group, which contains every host
- [module] = discrete units of code

## Grouping host

Track:

- WHERE - a datacenter/region
- WHAT - e.g. db, server etc
- WHEN - wich stage. e.g. dev, test, prod env
