# pgstrom-ansible

 Automatically Setup PG-Strom with Ansible

## How to Use

- [Install the ansible-core](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html) on Your Clients.
- Configure the [Inventory](https://docs.ansible.com/ansible/latest/getting_started/index.html). 
- You can also configure sudo users who do not need to provide any password by using the NOPASSWD option in the /etc/sudoers file.

```shell
#RHEL and RHEL clones
%wheel  ALL=(ALL)       NOPASSWD: ALL 

#Debian and Ubuntu
%sudo  ALL=(ALL)       NOPASSWD: ALL 
```

- And...

```shell
ansible-playbook playbook.yaml -i hosts.ini
```

## Version

You can set up with the following configuration.

| OSVer | KernelVer | CUDAVer |
| --- | --- | --- |
| Red Hat Enterprise Linux 8.6 | 4.18.0-372.32.1.el8_6.x86_64 | 12.0.1 |
| Red Hat Enterprise Linux 8.8 | >= 4.18.0-477 | 12.2 |
| Rocky Linux 8.7 | >= 4.18.0-425 | 12.1 |
| Rocky Linux 8.8 | >= 4.18.0-477 | 12.2 |
