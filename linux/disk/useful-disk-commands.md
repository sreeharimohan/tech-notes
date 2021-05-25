# Useful Disk Commands
## mount
```
$ mount
/dev/sda3 on / type ext4 (rw,errors=remount-ro)
proc on /proc type proc (rw,noexec,nosuid,nodev)
sysfs on /sys type sysfs (rw,noexec,nosuid,nodev)
...
/dev/mapper/lvmg-homelvm on /home type btrfs (rw,relatime,compress=lzo,space_cache)
/dev/sda5 on /home/muru/arch type btrfs (rw,relatime,compress=lzo,space_cache)
binfmt_misc on /proc/sys/fs/binfmt_misc type binfmt_misc (rw,noexec,nosuid,nodev)
systemd on /sys/fs/cgroup/systemd type cgroup (rw,noexec,nosuid,nodev,none,name=systemd)
```
## df
```
$ df
Filesystem                1K-blocks      Used Available Use% Mounted on
/dev/sda3                  30832636  11993480  17249912  42% /
none                              4         0         4   0% /sys/fs/cgroup
...
/dev/sda5                  31457280   3948600  25396496  14% /mnt/resources
```
## lsblk
```
$ lsblk
NAME   MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
sdb      8:16   0  200G  0 disk
└─sdb1   8:17   0  200G  0 part /mnt/resource
sda      8:0    0  500G  0 disk
└─sda1   8:1    0  500G  0 part /
```