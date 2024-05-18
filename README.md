# My Proxmox notes
Snippets about Proxmox.

## Media
### lxc bind mount:
Create directory in host, best if in /mnt/bindmounts.
`pct set {lxc num} -mp0 /mnt/bindmounts/{hostdir},mp=/{lxcdir}`
