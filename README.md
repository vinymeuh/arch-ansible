# arch-ansible

A set of [Ansible](https://www.ansible.com/) playbooks to setup and manage [Arch Linux](https://archlinux.org/) on computers.

## Bootstrap

1. Install [Arch Linux](https://github.com/vinymeuh/arch-ansible/blob/master/docs/INSTALL-ARCHLINUX.md)

2. Install **pyenv** using [pyenv installer](https://github.com/pyenv/pyenv-installer)

3. Create Python **virtualenv**:

```shell
pyenv virtualenv system arch-ansible
```

4. Install Ansible

```shell
cd $HOME
git clone https://github.com/vinymeuh/arch-ansible
cd arch-ansible
pyenv version  # must be arch-ansible, see .python-version
pip install -r requirements.txt
```

5. Install Ansible collections


```shell
ansible-galaxy collection install -r requirements.yml
```
