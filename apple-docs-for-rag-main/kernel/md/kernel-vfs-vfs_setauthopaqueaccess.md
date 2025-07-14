

- Kernel
- vfs
-  vfs_setauthopaqueaccess 

Function

# vfs_setauthopaqueaccess

Mark a filesystem as having remote VNOP_ACCESS support.

macOS 10.4+

``` source
void vfs_setauthopaqueaccess(mount_t mp);
```

## Parameters 

`mp`  

Mount to mark.

## Return Value

void.

