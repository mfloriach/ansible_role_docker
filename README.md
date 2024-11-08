# Ansible role for installing wordpres with docker compose

Ansible role to install wordpress in a ubuntu machine using docker compose.

## Install
Edit the `nodes.ini` with the server credentials and add the `ssh_key` on the keys folder.

## Run
```
$ ansible all -m ping -i nodes.ini
$ ansible-playbook -i nodes.ini nodes.yaml -K
```

## Trobleshooting
Do not forget to add the public key on the servers with the following command:
```
ssh-copy-id <USERNAME>@<IP>
```