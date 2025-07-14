

- Kernel
- vfs
-  vfs_fsprivate 

Function

# vfs_fsprivate

Get filesystem-private mount data.

macOS 10.4+

``` source
void * vfs_fsprivate(mount_t mp);
```

## Parameters 

`mp`  

Mount for which to get private data.

## Return Value

Private data.

## Discussion

A filesystem generally has an internal mount structure which it attaches to the VFS-level mount structure as part of the mounting process.

