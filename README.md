# JHipster Ansible

## Prerequisites

You have to install Ansible:

```
sudo apt-add-repository -y ppa:ansible/ansible && \
sudo apt-get update && \
sudo apt-get install -y ansible
```

## Roles for Releases

### jhipster lib

To prepare locally the release:

```
ansible-playbook -vvv playbooks/jhipster-prepare.yml
```

To publish the release:

```
ansible-playbook -vvv playbooks/jhipster-release.yml
```

### generator-jhipster

To prepare locally the release:

```
ansible-playbook -v playbooks/generator-jhipster-prepare.yml
```

To publish the release:

```
ansible-playbook -v playbooks/generator-jhipster-release.yml
```
