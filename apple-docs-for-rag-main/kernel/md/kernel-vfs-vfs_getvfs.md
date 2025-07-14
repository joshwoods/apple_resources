

- Kernel
- vfs
-  vfs_getvfs 

Function

# vfs_getvfs

Given a filesystem ID, look up a mount structure.

macOS 10.4+

``` source
mount_t vfs_getvfs(fsid_t *fsid);
```

## Parameters 

`fsid`  

Filesystem ID to look up.

## Return Value

Mountpoint if found, else NULL. Note unmounting mountpoints can be returned.

