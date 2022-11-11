Ansible setup

### Run in docker

```sh
docker build -t ansible .
docker run --rm -it ansible bash
ansible-playbook default.yml --ask-vault-pass
```

### Run in pop-os

```sh
ansible-playbook default.yml --ask-vault-pass --ask-become-pass
```

### Run in mac-os

1. Ensure Apple's command line tools are installed (xcode-select --install to launch the installer).

2. Install Ansible:

 - Run the following command to add Python 3 to your $PATH: export PATH="$HOME/Library/Python/3.8/bin:/opt/homebrew/bin:$PATH"
 - Upgrade Pip: sudo pip3 install --upgrade pip
 - Install Ansible: pip3 install ansible

3. Clone or download this repository to your local drive.

4. Run ansible-galaxy install -r requirements.yml inside this directory to install required Ansible roles.

5. Run ansible-playbook mac.yml -i inventory --ask-become-pass inside this directory. Enter your macOS account password when prompted for the 'BECOME' password.


