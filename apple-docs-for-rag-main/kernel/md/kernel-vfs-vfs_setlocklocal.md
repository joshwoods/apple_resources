

- Kernel
- vfs
-  vfs_setlocklocal 

Function

# vfs_setlocklocal

Mark a filesystem as using VFS-level advisory locking support.

macOS 10.4+

``` source
void vfs_setlocklocal(mount_t mp);
```

## Parameters 

`mp`  

Mount to mark.

## Return Value

void.

## Discussion

Advisory locking operations will not call down to the filesystem if this flag is set.

