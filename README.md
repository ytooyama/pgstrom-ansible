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
| Rocky Linux 8.10 | >= 4.18.0-553 | 13.1.1 |
| Rocky Linux 9.7 | >= 5.14.0-611.5 | 13.1.1 |
| Rocky Linux 10.1 | >= 6.12.0-124 | 13.1.1 |
| AlmaLinux 8.10 | >= 4.18.0-553 | 13.1.1 |
| AlmaLinux 9.7 | >= 5.14.0-611.5 | 13.1.1 |
| Rocky Linux 10.1 | >= 6.12.0-124 | 13.1.1 |

