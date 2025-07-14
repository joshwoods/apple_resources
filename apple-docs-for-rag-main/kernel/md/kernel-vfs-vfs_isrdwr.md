

- Kernel
- vfs
-  vfs_isrdwr 

Function

# vfs_isrdwr

Determine if a filesystem is mounted with writes enabled.

macOS 10.4+

``` source
int vfs_isrdwr(mount_t mp);
```

## Parameters 

`mp`  

Mount to test.

## Return Value

Nonzero if filesystem is mounted read-write, else 0.

