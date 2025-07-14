

- Kernel
- vfs
-  vfs_setauthopaque 

Function

# vfs_setauthopaque

Mark a filesystem as having authorization decisions controlled remotely.

macOS 10.4+

``` source
void vfs_setauthopaque(mount_t mp);
```

## Parameters 

`mp`  

Mount to mark.

## Return Value

void.

