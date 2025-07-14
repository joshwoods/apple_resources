

- Kernel
- vfs
-  vfs_statfs 

Function

# vfs_statfs

Get information about filesystem status.

macOS 10.4+

``` source
struct vfsstatfs * vfs_statfs(mount_t mp);
```

## Parameters 

`mp`  

Mount for which to get vfsstatfs pointer.

## Return Value

Pointer to vfsstatfs.

## Discussion

Each filesystem has a struct vfsstatfs associated with it which is updated as events occur; this function returns a pointer to it. Note that the data in the structure will continue to change over time and also that it may be quite stale of vfs_update_vfsstat has not been called recently.

