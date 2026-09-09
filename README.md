# AWS Ansible Webservers

This project deploys Nginx webservers on two Ubuntu EC2 virtual machines using Ansible.

## Server Results

VM1 displays:

Hello World from SJSU-1

VM2 displays:

Hello World from SJSU-2

## Files

- inventory.ini: Ansible host inventory
- deploy.yml: Deploys Nginx and the website
- undeploy.yml: Removes Nginx and website resources
- templates/index.html.j2: Website template

## Commands

Test connectivity:

```bash
ansible all -i inventory.ini -m ping
