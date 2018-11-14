# Prometheus with AlertManager using Ansible

In this project, we are configurating prometheus, node_exporter with alertmanager. We track "up" state of node_exporter instance and if instance goes down prometheus trigger an alert to alertmanager which is fired to slack.

## Getting Started

Step 1: Update slack webhook slack_api_url param in alermanager template file alertmanager.yml.j2 

Step 2: Update ip address of instances in inventory file.

Step 3: Run ansible command to setup prometheus, node_exporter and alertmanager services

Ansible command: ansible-playbook playbook.yml
