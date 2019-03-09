# Ansible Role: Docker Service

Simple docker installation on CentOS-7 with adjustments for running via ansible.

Based on:

- https://docs.docker.com/install/linux/docker-ce/centos/#install-using-the-repository


## Requirements

N/A


## Role Variables

Please look at: ``defaults/main.yml``
 

## Dependencies

N/A


## Installation

### Directly from ansible-galaxy (latest release)

```bash
$ ansible-galaxy install marcinpraczko.docker_service
```

### Directly from github repository

Sometimes some changes has been applied to ``develop`` or ``feature`` branch and are not yet released.
Ansible-galaxy allows install roles directly from ``GitHub``.

```bash
ansible-galaxy install -p roles git+https://github.com/marcinpraczko/ansible-role-docker_service.git,develop
```

Above example will install ``develop`` branch. This can be adjusted to any git SHA commit, tag or branch
name - depends of requirements.

Checking what version is installed can be done with command:
```bash
ansible-galaxy list -p roles
```


### Via Ansible-Galaxy in requirements.yml

```yaml
- src: marcinpraczko.docker_service
  name: "marcinpraczko.docker_service"
  version: 0.1.0
```

## Example Playbook

```yaml
- hosts: servers
  roles:
    - { role: "marcin.praczko.docker_service" }
```


## License

MIT / BSD


## Author Information

Marcin Praczko
