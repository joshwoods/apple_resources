

- Kernel
- vfs
-  vfs_setfsprivate 

Function

# vfs_setfsprivate

Set filesystem-private mount data.

macOS 10.4+

``` source
void vfs_setfsprivate(mount_t mp, void *mntdata);
```

## Parameters 

`mp`  

Mount for which to set private data.

## Return Value

Void.

## Discussion

A filesystem generally has an internal mount structure which it attaches to the VFS-level mount structure as part of the mounting process.

