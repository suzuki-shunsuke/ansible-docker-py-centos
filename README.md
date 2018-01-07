# ansible-docker-py-centos

ansible role to install docker-py on CentOS

https://galaxy.ansible.com/suzuki-shunsuke/docker-py-centos/

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
