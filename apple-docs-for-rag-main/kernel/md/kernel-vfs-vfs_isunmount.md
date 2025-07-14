

- Kernel
- vfs
-  vfs_isunmount 

Function

# vfs_isunmount

Determine if an unmount is in progress.

macOS 10.6+

``` source
int vfs_isunmount(mount_t mp);
```

## Parameters 

`mp`  

Mount to test.

## Return Value

Nonzero if an unmount is in progress, else zero.

## Discussion

This is an unsynchronized snapshot of the mount state. It should only be called if the mount is known to be valid, e.g. there are known to be live files on that volume.

