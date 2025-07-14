

- Kernel
- vfs
-  vfs_devblocksize 

Function

# vfs_devblocksize

Get the block size of the device underlying a mount.

macOS 10.4+

``` source
int vfs_devblocksize(mount_t mp);
```

## Parameters 

`mp`  

Mount for which to get block size.

## Return Value

Block size.

