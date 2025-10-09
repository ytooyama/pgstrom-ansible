# pgstrom-ansible

 Automatically Setup PG-Strom with Ansible

## How to Use

- [Install the ansible-core](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) on Your Clients.
- Configure the [Inventory](https://docs.ansible.com/ansible/latest/getting_started/index.html). 
- You can also configure sudo users who do not need to provide any password by using the NOPASSWD option in the /etc/sudoers file.

```shell
#RHEL and RHEL clones
%wheel  ALL=(ALL)       NOPASSWD: ALL 
```

- And...

```shell
ansible-playbook playbook.yaml -i hosts.ini
```

## Version

You can set up with the following configuration.

| OSVer | KernelVer | CUDAVer |
| --- | --- | --- |
| Rocky Linux 9.6 | >= 5.14.0-503 | 12.9.1 |
| AlmaLinux 9.6 | >= 5.14.0-503 | 12.9.1 |