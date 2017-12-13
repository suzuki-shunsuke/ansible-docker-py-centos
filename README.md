# ansible-docker-py-centos

ansible role to install docker-py on CentOS

https://galaxy.ansible.com/suzuki-shunsuke/docker-py-centos/

## Requirements

Nothing.

## Role Variables

Nothing.

## Dependencies

* [geerlingguy.repo-epel](https://galaxy.ansible.com/geerlingguy/repo-epel/)

## Example Playbook

```yaml
- hosts: servers
  roles:
    - role: suzuki-shunsuke.docker-py-centos
      become: yes
```

## License

[MIT](LICENSE)
