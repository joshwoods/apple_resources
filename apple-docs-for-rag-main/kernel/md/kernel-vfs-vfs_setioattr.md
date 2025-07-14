

- Kernel
- vfs
-  vfs_setioattr 

Function

# vfs_setioattr

Set I/O attributes associated with a mounpoint.

macOS 10.4+

``` source
void vfs_setioattr(mount_t mp, struct vfsioattr *ioattrp);
```

## Parameters 

`mp`  

Mount for which to set attributes.

`ioattrp`  

Structure containing I/O parameters; all fields must be filled in.

## Return Value

void.

