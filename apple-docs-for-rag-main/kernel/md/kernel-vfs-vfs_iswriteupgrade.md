

- Kernel
- vfs
-  vfs_iswriteupgrade 

Function

# vfs_iswriteupgrade

Determine if a filesystem is mounted read-only but a request has been made to upgrade to read-write.

macOS 10.4+

``` source
int vfs_iswriteupgrade(mount_t mp);
```

## Parameters 

`mp`  

Mount to test.

## Return Value

Nonzero if a request has been made to update from read-only to read-write, else 0.

