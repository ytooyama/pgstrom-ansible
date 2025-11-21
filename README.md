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
ansible-playbook playbook.yaml -i hosts.ini -l home
```

## Support Versions
You can set up with the following configuration.

### Stable
 
| OSVer | KernelVer | CUDAVer |
| --- | --- | --- |
| Rocky Linux 8.10 | >= 4.18.0-553 | 13.0.2 |
| Rocky Linux 9.6 | >= 5.14.0-570.17.1 | 13.0.2 |
| Rocky Linux 10.0 | >= 6.12.0-55.12.1 | 13.0.2 |
| AlmaLinux 8.10 | >= 4.18.0-553 | 13.0.2 |
| AlmaLinux 9.6 | >= 6.12.0-55.12.1 | 13.0.2 |

### Legacy

| OSVer | KernelVer | CUDAVer |
| --- | --- | --- |
| Rocky Linux 9.6 | >= 5.14.0-503 | 13.0.2 |
| AlmaLinux 9.6 | >= 5.14.0-503 | 13.0.2 |
