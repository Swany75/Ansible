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

```bash
ansible-playbook playbooks/ping.yml
```

## Disclaimer!

Som conscient de que no es recomanable compartir les claus, pero aquestes no tenen cap valor, son per fer proves.
