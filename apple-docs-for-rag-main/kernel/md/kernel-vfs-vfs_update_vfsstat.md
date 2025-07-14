

- Kernel
- vfs
-  vfs_update_vfsstat 

Function

# vfs_update_vfsstat

Update cached filesystem status information in the VFS mount structure.

macOS 10.4+

``` source
int vfs_update_vfsstat(mount_t mp, vfs_context_t ctx, int eventtype);
```

## Parameters 

`mp`  

Mount for which to update cached status information.

`ctx`  

Context to authenticate against for call down to filesystem.

`eventtype`  

VFS_USER_EVENT: need for update is driven by user-level request; perform additional authentication. VFS_KERNEL_EVENT: need for update is driven by in-kernel events. Skip extra authentication.

## Return Value

0 for success, or an error code for authentication failure or problem with call to filesystem to request information.

## Discussion

Each filesystem has a struct vfsstatfs associated with it which is updated as events occur; this function updates it so that the structure pointer returned by vfs_statfs() returns a pointer to fairly recent data.

