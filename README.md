# Personal Linux setup using Ansible

```shell
sudo add-apt-repository ppa:ansible/ansible
sudo apt-get update
sudo apt-get install ansible git
ansible-playbook setup.yml --ask-become-pass
```

## Tags
```
  tags:
    - docker

```

```shell

ansible-playbook setup.yml --ask-become-pass --tags "docker"
```


## Upgrade to new Ubuntu Version
Remove all the files in `/etc/apt/sources.list.d/` and then run the playbook.
Otherwise the upgrade comments out 3rd party repos
