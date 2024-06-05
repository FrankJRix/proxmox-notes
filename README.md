# My Proxmox notes
Snippets about Proxmox.

## Markdown reference

[Here.](https://www.markdownguide.org/cheat-sheet/)

## Copypaste

`code here`

## Administration
### update system:
`apt update`\
`apt dist-upgrade`

## Media
### lxc bind mount:
Create directory in host and then

`pct set {lxc num} -mp{N} /mnt/.../{hostdir},mp=/mnt/{lxcdir}`

#### if you want to be unsafe:
edit permissions to 777!

`chmod -R 777 /mnt/bindmounts/{hostdir}`

#### if you want to be safe:

TBA

## Hardware
### usb drive smart status:

`man smartd`\
`man smartd.conf`

`systemtcl -d sat /dev/sdx`

### usb quirks:
if a drive isn't recognized in the disk section, get the problem disk id with
`lsusb`

id = xxxx:xxxx

`echo options usb-storage quirks=xxxx:xxxx:u | tee /etc/modprobe.d/blacklist_uas.conf`\
`update-initramfs -u`

and then you reboot.
