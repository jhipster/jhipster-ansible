# JHipster Ansible

## Prerequisites

### Ansible

You have to install Ansible:

```
sudo apt-add-repository -y ppa:ansible/ansible && \
sudo apt-get update && \
sudo apt-get install -y ansible
```

Or, if you prefer Homebrew:

```
brew install ansible
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

### jhipster-bom

To prepare locally the release:

```
ansible-playbook -v playbooks/jhipster-bom-prepare.yml
```

To publish the release:

```
ansible-playbook -v playbooks/jhipster-bom-release.yml
```


### react-jhipster

To prepare locally the release:

```
ansible-playbook -v playbooks/react-jhipster-prepare.yml
```

To publish the release:

```
ansible-playbook -v playbooks/react-jhipster-release.yml
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

### documentation-archive

To prepare locally the release:

```
ansible-playbook -v playbooks/documentation-archive-prepare.yml
```

To publish the release:

```
ansible-playbook -v playbooks/documentation-archive-release.yml
```


### jhipster-control-center

To prepare locally the release:

```
ansible-playbook -v playbooks/jhcc-prepare.yml
```

To publish the release:

```
ansible-playbook -v playbooks/jhcc-release.yml
```
