# Playbooks
My Ansible Playbooks

## Abans de res: Instal·la Ansible

```bash
apt install ansible
```

## Envia la clau publica als hosts

```bash
ssh-copy-id -i keys/ansible-key.pub root@{IP}
```

## Executar un Playbook

Playbook ping

```bash
ansible-playbook playbooks/ping.yml
```

Playbook Update

```bash
ansible-playbook playbooks/update.yml
```

Playbook Create Zone

```bash
ansible-playbook playbooks/createzone.yml -e "hostDNS=SVR-DNS hostWEB=SVR-WEB zonename=exemple.com"
```

Playbook Create VirtualHost

```bash
ansible-playbook playbooks/createvhost.yml -e "zone=ies.cat DNS=SVR-DNS WEB=SVR-WEB"
```

## Disclaimer!

Som conscient de que no es recomanable compartir les claus, pero aquestes no tenen cap valor, son per fer proves.
