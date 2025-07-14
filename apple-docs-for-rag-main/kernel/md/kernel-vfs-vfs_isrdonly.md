

- Kernel
- vfs
-  vfs_isrdonly 

Function

# vfs_isrdonly

Determine if a filesystem is mounted read-only.

macOS 10.4+

``` source
int vfs_isrdonly(mount_t mp);
```

## Parameters 

`mp`  

Mount to test.

## Return Value

Nonzero if filesystem is mounted read-only, else 0.

