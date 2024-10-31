# [btrfs-progs-gael](https://snapcraft.io/btrfs-progs-gael)

_This is NOT an original piece of work, just a snap of btrfs-progs_

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
sudo snap install btrfs-progs-gael_v6.6.3_amd64.snap --devmode

sudo snap alias btrfs-progs-gael.btrfs btrfs
sudo snap alias btrfs-progs-gael.mkfs-btrfs mkfs.btrfs
sudo snap alias btrfs-progs-gael.btrfs-snap btrfs-snap
sudo snap alias btrfs-progs-gael.btrfs-scrub btrfs-scrub
```

**Scrubbing**

* Results stored in $SNAP_DATA/var/lib/btrfs
