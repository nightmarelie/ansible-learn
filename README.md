## Ansible ad-hoc commands

> ansible [pattern] -m [module] -a "[module options]"

- [pattern] = targeting hosts and groups
  - "all" = default group, which contains every host
- [module] = discrete units of code

Example:

> ansible all -i hosts -m ping

> ansible droplet -i hosts -m ping

## Grouping host

Track:

- WHERE - a datacenter/region
- WHAT - e.g. db, server etc
- WHEN - wich stage. e.g. dev, test, prod env

## Ansible playbook

> ansible-playbook -i hosts app-playbook.yaml
> ansible-playbook -i inventory_aws_ec2.yaml deploy-docker-ec2-user.yaml

## Ansible inventory

> ansible-inventory -i inventory_aws_ec2.yaml --graph
