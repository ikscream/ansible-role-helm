# ansible-role-helm
Ansible role for installing helm on linux

1. Create role reference in your `requirements.yml` file:

```shell
- name: ansible-role-helm
  src: https://github.com/ikscream/ansible-role-helm.git
  version: main
```

2. Install remote role with `ansible-galaxy`:

```shell
ansible-galaxy install -r requirements.yml
```

3. Use role inside playbook:

```shell
- hosts: localhost
  become: true
  gather_facts: no
  roles:
    - ansible-role-helm
```
