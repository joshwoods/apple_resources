

- Kernel
- vfs
-  vfs_clearauthopaqueaccess 

Function

# vfs_clearauthopaqueaccess

Mark a filesystem as not having remote VNOP_ACCESS support.

macOS 10.4+

``` source
void vfs_clearauthopaqueaccess(mount_t mp);
```

## Parameters 

`mp`  

Mount to mark.

## Return Value

void.

