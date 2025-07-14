

- Kernel
- vfs
-  vfs_fsadd 

Function

# vfs_fsadd

Register a filesystem with VFS.

macOS 10.4+

``` source
int vfs_fsadd(struct vfs_fsentry *vfe, vfstable_t *handle);
```

## Parameters 

`vfe`  

Filesystem information: table of vfs operations, list of vnode operation tables, filesystem type number (can be omitted with VFS_TBLNOTYPENUM flag), name, flags.

`handle`  

Opaque handle which will be passed to vfs_fsremove.

## Return Value

0 for success, else an error code.

## Discussion

Typically called by a filesystem Kernel Extension when it is loaded.

