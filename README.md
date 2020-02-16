# JHipster Ansible

## Prerequisites

### Ansible

You have to install Ansible:

```
sudo apt-add-repository -y ppa:ansible/ansible && \
sudo apt-get update && \
sudo apt-get install -y ansible
```

### Projects

Before cloning a project, be sure you already forked it, under GitHub.
Then, all projects are cloned with:
- `origin`: your fork
- `upstream`: the original project


## Roles for cloning project

### Clone single repository

```
ansible-playbook -v playbooks/clone-fork.yml
```

### Clone JHipster projects

```
ansible-playbook -v playbooks/clone-jhipster-projects.yml
```


## Roles for Releases

### jhipster lib

To prepare locally the release:

```
ansible-playbook -v playbooks/jhipster-prepare.yml
```

To publish the release:

```
ansible-playbook -v playbooks/jhipster-release.yml
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

### jhipster-vuejs

To prepare locally the release:

```
ansible-playbook -v playbooks/jhipster-vuejs-prepare.yml
```

To publish the release:

```
ansible-playbook -v playbooks/jhipster-vuejs-release.yml
```
