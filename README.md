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

To prepare locally the release:

```
ansible-playbook -v playbooks/jhipster-prepare.yml
```

To publish the release:

```
ansible-playbook -v playbooks/jhipster-release.yml
```
