# JHipster Ansible

## Prerequisites

You have to install Ansible:

```
sudo apt-add-repository -y ppa:ansible/ansible && \
sudo apt-get update && \
sudo apt-get install -y ansible
```

## Roles for Releases

### jhipster

```
ansible-playbook -v playbooks/jhipster.yml
```