

- Kernel
- vfs
-  vfs_issynchronous 

Function

# vfs_issynchronous

Determine if writes to a filesystem occur synchronously.

macOS 10.4+

``` source
int vfs_issynchronous(mount_t mp);
```

## Parameters 

`mp`  

Mount to test.

## Return Value

Nonzero if writes occur synchronously, else 0.

