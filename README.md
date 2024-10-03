# ITLab

home lab for hosting services like databases, media servers, wordpress. Learning and experimentation with IT stuff proxmox ve became my go-to solution for provision VMs. I automated most of the things with ansible so that I can rebuild my lab in any case of hardware failure with few commands.

## Nodes

1. **databases**

I mostly use postgres, mariadb, and mongodb. I needed web UI to manage those dbs I chose adminer to manage postgres and mariadb and mongo-express for mongodb. All databases are installed through docker as docker images.

2. **files & media server**

I like samba for its simplicity of setup and use, I also use jellyfin to host medias.

3. **nextcloud**

I wanted to have a self-hosted office suite to manage documents, spreadsheets, and presentations from my browser. I would like to look for other features in the future.

## How to setup

```sh
ansible-playbook ./playbooks/{{playbook_file}}.yml -i inventory --user={{username}} -kK
```
## Contributing

Doors for any kind of support and contribution are opened.
