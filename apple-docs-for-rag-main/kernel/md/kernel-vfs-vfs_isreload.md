

- Kernel
- vfs
-  vfs_isreload 

Function

# vfs_isreload

Determine if a reload of filesystem data is in progress. This can only be the case for a read-only filesystem; all data is brought in from secondary storage.

macOS 10.4+

``` source
int vfs_isreload(mount_t mp);
```

## Parameters 

`mp`  

Mount to test.

## Return Value

Nonzero if a request has been made to reload data, else 0.

