

- Kernel
- vfs
-  vfs_attr_pack_ext 

Function

# vfs_attr_pack_ext

macOS 10.15+

``` source
errno_t vfs_attr_pack_ext(mount_t mp, vnode_t vp, uio_t uio, struct attrlist *alp, uint64_t options, struct vnode_attr *vap, void *fndesc, vfs_context_t ctx);
```

