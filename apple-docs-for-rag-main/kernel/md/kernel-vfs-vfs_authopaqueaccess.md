

- Kernel
- vfs
-  vfs_authopaqueaccess 

Function

# vfs_authopaqueaccess

Check if a filesystem is marked as having reliable remote VNOP_ACCESS support.

macOS 10.4+

``` source
int vfs_authopaqueaccess(mount_t mp);
```

## Parameters 

`mp`  

Mount to test.

## Return Value

Nonzero if VNOP_ACCESS is supported remotely, else 0.

