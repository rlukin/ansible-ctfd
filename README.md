# ansible-ctfd
Ansible playbook for deploying [CTFd](https://github.com/CTFd/CTFd)

## How to deploy
* Change ```inventory``` file
* Give it a shot with:
```bash
ansible-playbook -i inventory -e enable_ssl=true site.yml 
```
### SSL
Don't forget to point your A records to server ip
### Notes
Was deployed on top of:
```bash
root@ubuntu-s-1vcpu-1gb-nyc1-01:~# tail /etc/*release
==> /etc/lsb-release <==
DISTRIB_ID=Ubuntu
DISTRIB_RELEASE=16.04
DISTRIB_CODENAME=xenial
DISTRIB_DESCRIPTION="Ubuntu 16.04.5 LTS"

==> /etc/os-release <==
VERSION="16.04.5 LTS (Xenial Xerus)"
ID=ubuntu
ID_LIKE=debian
PRETTY_NAME="Ubuntu 16.04.5 LTS"
VERSION_ID="16.04"
HOME_URL="http://www.ubuntu.com/"
SUPPORT_URL="http://help.ubuntu.com/"
BUG_REPORT_URL="http://bugs.launchpad.net/ubuntu/"
VERSION_CODENAME=xenial
UBUNTU_CODENAME=xenial
```

Happy hacking!
