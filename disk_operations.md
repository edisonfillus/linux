### List disk space 
```shell
df -h
```

### List partitions
```shell
fdisk -l
```

### Create a partition
```shell
fdisk /dev/dev_name
```
commands:
* p: print
* n: new
* w: write to disk

### Format
```shell
mkfs.ext4 /dev/partition_name
```

### Mount
```shell
mount /dev/partition_name /folder_name
```

### Include in /etc/fstab
```shell
/dev/partition_name  /folder_name ext4 defaults 0 2
```

### Create a symbolic link
```shell
sudo ln -s /destiny origin
```