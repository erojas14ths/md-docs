# Mount external disc

I. Create the mount point

For example, use drive folder.

`sudo mkdir /media/drive`

II. List folder

`ls -la /media/drive`

III. List disc  
Identifier your external disc.

For example. use sdb/sdb1

`lsblk`

IV. Identifier UUID Disk

`sudo blkid`

Show: Use UUID

`dev/sdb1: LABEL="your-external-drive" BLOCK_SIZE="512" UUID="6666BA9166BA620B" TYPE="ntfs" PARTUUID="26a8d186-01"`  

V. Edit config mount disk

`UUID=6666BA9166BA620B /media/drive ntfs defaults 0 0`

VI. Reboot