

- Kernel
- vfs
-  vfs_fsremove 

Function

# vfs_fsremove

Unregister a filesystem with VFS.

macOS 10.4+

``` source
int vfs_fsremove(vfstable_t handle);
```

## Parameters 

`handle`  

Handle which was returned by vfs_fsadd.

## Return Value

0 for success, else an error code.

## Discussion

Typically called by a filesystem Kernel Extension when it is unloaded.

