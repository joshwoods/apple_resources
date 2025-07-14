

- Kernel
- vfs
-  vfs_removename 

Function

# vfs_removename

Deprecated

macOS 10.4+

``` source
int vfs_removename(const char *name);
```

## Discussion

vnode_update_identity() and vnode_create() make vfs_addname() unnecessary for kexts.

