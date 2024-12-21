# arch-ansible

A set of [Ansible](https://www.ansible.com/) playbooks to setup and manage [Arch Linux](https://archlinux.org/) on my computers.

## Bootstrap

1. Install [Arch Linux](https://github.com/vinymeuh/arch-ansible/blob/master/docs/INSTALL-ARCHLINUX.md)

2. Install **python-pipx**

3. Install Ansible

```shell
cd $HOME
git clone https://github.com/vinymeuh/arch-ansible
cd arch-ansible
echo $PIPX_BIN_DIR # must be ~/bin
pipx install ansible-core
```

4. Install Ansible collections

```shell
ansible-galaxy collection install -r requirements.yml
```

## Usage

```shell
ansible-playbook playbooks/nyx-system.yml -K --check
ansible-playbook playbooks/nyx-system.yml --list-tags
```
