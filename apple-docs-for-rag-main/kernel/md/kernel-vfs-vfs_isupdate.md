

- Kernel
- vfs
-  vfs_isupdate 

Function

# vfs_isupdate

Determine if a mount update is in progress.

macOS 10.4+

``` source
int vfs_isupdate(mount_t mp);
```

## Parameters 

`mp`  

Mount to test.

## Return Value

Nonzero if a mount update is in progress, 0 otherwise.

