

- Kernel
- Kernel Data Types
- vfsops
-  vfs_fhtovp 

Instance Property

# vfs_fhtovp

macOS 10.6+

``` source
int (*vfs_fhtovp)(struct mount *mp, int fhlen, unsigned char *fhp, struct vnode **vpp, vfs_context_t context);
```

