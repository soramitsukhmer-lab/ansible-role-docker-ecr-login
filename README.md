# ansible-role-docker-ecr-login
Ansible Role - Docker Login for Amazon ECR

## Role Variables
Available variables are listed below, along with default values (see `defaults/main.yml`):

```yml
aws_access_key: "key"
aws_secret_key: "secret"
aws_region: "ap-southeast-1"

aws_ecr_registry: "012345678912.dkr.ecr.ap-southeast-1.amazonaws.com"
```

## Use with Ansible

Example:

```yml
- hosts: all

  vars:
    pip_install_packages:
      - name: docker
      - name: jsondiff

  roles:
    - soramitsukhmer-lab.pip
    - soramitsukhmer-lab.docker
    - soramitsukhmer-lab.docker-ecr-login
```
