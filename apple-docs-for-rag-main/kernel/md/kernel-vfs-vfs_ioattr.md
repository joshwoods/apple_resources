

- Kernel
- vfs
-  vfs_ioattr 

Function

# vfs_ioattr

Get I/O attributes associated with a mounpoint.

macOS 10.4+

``` source
void vfs_ioattr(mount_t mp, struct vfsioattr *ioattrp);
```

## Parameters 

`mp`  

Mount for which to get attributes. If NULL, system defaults are filled into ioattrp.

`ioattrp`  

Destination for results.

## Return Value

void.

