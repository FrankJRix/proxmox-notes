# My Proxmox notes
Snippets about Proxmox.

## Markdown reference

[Here.]([https://www.example.com](https://www.markdownguide.org/cheat-sheet/))

## Copypaste

`code here`

## Media
### lxc bind mount:
Create directory in host, best if in /mnt/bindmounts, and then

`pct set {lxc num} -mp0 /mnt/bindmounts/{hostdir},mp=/{lxcdir}`

edit permissions to 777!

`chmod -R 777 /mnt/bindmounts/{hostdir}`
