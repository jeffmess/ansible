Ansible setup

### Run in docker

```sh
docker build -t ansible .
docker run --rm -it ansible bash
ansible-playbook default.yml --ask-vault-pass
```

### Run in pop-os

```sh
ansible-playbook default.yml --ask-vault-pass --ask-pass
```
