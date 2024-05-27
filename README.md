# My Proxmox notes
Snippets about Proxmox.

## Markdown reference

[Here.](https://www.markdownguide.org/cheat-sheet/)

## Copypaste

`code here`

## Administration
### update system:
`apt update`
`apt dist-upgrade`

## Media
### lxc bind mount:
Create directory in host, best if in /mnt/bindmounts, and then

`pct set {lxc num} -mp0 /mnt/bindmounts/{hostdir},mp=/{lxcdir}`

#### if you want to be unsafe:
edit permissions to 777!

`chmod -R 777 /mnt/bindmounts/{hostdir}`

#### if you want to be safe:

TBA
