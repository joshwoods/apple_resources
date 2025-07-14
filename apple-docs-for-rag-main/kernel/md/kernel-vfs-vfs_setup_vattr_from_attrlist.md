

- Kernel
- vfs
-  vfs_setup_vattr_from_attrlist 

Function

# vfs_setup_vattr_from_attrlist

macOS 10.10+

``` source
errno_t vfs_setup_vattr_from_attrlist(struct attrlist *alp, struct vnode_attr *vap, enum vtype obj_vtype, ssize_t *attr_fixed_sizep, vfs_context_t ctx);
```

