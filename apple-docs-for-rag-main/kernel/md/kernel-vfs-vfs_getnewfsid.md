

- Kernel
- vfs
-  vfs_getnewfsid 

Function

# vfs_getnewfsid

Generate a unique filesystem ID for a mount and store it in the mount structure.

macOS 10.4+

``` source
void vfs_getnewfsid(struct mount *mp);
```

## Parameters 

`mp`  

Mount to set an ID for.

## Return Value

void.

## Discussion

Filesystem IDs are returned as part of "struct statfs." This function is typically called as part of file-system specific mount code (i.e. through VFS_MOUNT).

