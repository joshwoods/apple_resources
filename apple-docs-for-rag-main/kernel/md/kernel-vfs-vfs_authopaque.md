

- Kernel
- vfs
-  vfs_authopaque 

Function

# vfs_authopaque

Determine if a filesystem's authorization decisions occur remotely.

macOS 10.4+

``` source
int vfs_authopaque(mount_t mp);
```

## Parameters 

`mp`  

Mount to test.

## Return Value

Nonzero if filesystem authorization is controlled remotely, else 0.

