

- Kernel
- Kernel Data Types
- vfsops
-  vfs_vptofh 

Instance Property

# vfs_vptofh

macOS 10.6+

``` source
int (*vfs_vptofh)(struct vnode *vp, int *fhlen, unsigned char *fhp, vfs_context_t context);
```

