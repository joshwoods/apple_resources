

- Kernel
- vfs
-  vfs_addname 

Function

# vfs_addname

Deprecated

macOS 10.4+

``` source
const char * vfs_addname(const char *name, uint32_t len, uint32_t nc_hash, uint32_t flags);
```

## Discussion

vnode_update_identity() and vnode_create() make vfs_addname() unnecessary for kexts.

