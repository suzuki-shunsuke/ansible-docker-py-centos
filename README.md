# ansible-docker-py-centos

[![Ansible Role](https://img.shields.io/ansible/role/22764.svg)](https://galaxy.ansible.com/suzuki-shunsuke/docker-py-centos/)
[![Ansible Role](https://img.shields.io/ansible/role/d/22764.svg)](https://galaxy.ansible.com/suzuki-shunsuke/docker-py-centos/)
[![GitHub last commit](https://img.shields.io/github/last-commit/suzuki-shunsuke/ansible-docker-py-centos.svg)](https://github.com/suzuki-shunsuke/ansible-docker-py-centos)

ansible role to install docker-py on CentOS

## Requirements

Nothing.

## Role Variables

name | required | default | example | description
--- | --- | --- | --- | ---
docker_py_python2_state | no | omit | latest | yum module's arguments
docker_py_pip_state | no | omit | latest | yum module's arguments
docker_py_docker_py_state | no | omit | latest | pip module's arguments

## Dependencies

* [geerlingguy.repo-epel](https://galaxy.ansible.com/geerlingguy/repo-epel/)

## Example Playbook

```yaml
- hosts: servers
  roles:
    - role: suzuki-shunsuke.docker-py-centos
      docker_py_docker_py_state: latest
      become: yes
```

## License

[MIT](LICENSE)
