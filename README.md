# [btrfs-progs-gael](https://snapcraft.io/btrfs-progs-gael)

btrfs is a modern copy on write (CoW) filesystem for Linux aimed at implementing advanced features while also focusing on fault tolerance, repair and easy administration. Its main features and benefits are:

* Snapshots which do not make the full copy of files
* RAID - support for software-based RAID 0, RAID 1, RAID 10
* Self-healing - checksums for data and metadata, automatic detection of silent data corruptions

For more information see: https://btrfs.wiki.kernel.org/

**Compile**

```bash
snapcraft --debug
```

**Install**

```bash
sudo snap install btrfs-progs-gael_5.11.1_amd64.snap --dangerous

sudo snap connect btrfs-progs-gael:block-devices
sudo snap connect btrfs-progs-gael:mount-observe
sudo snap connect btrfs-progs-gael:removable-media

sudo snap alias btrfs-progs-gael.btrfs btrfs
sudo snap alias btrfs-progs-gael.mkfs-btrfs mkfs.btrfs
```
