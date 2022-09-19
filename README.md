Ansible setup

### Run in docker

```sh
docker build -t ansible .
docker run --rm -it ansible bash
ansible-playbook default.yml
```
