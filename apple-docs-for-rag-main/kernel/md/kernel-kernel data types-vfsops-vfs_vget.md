

- Kernel
- Kernel Data Types
- vfsops
-  vfs_vget 

Instance Property

# vfs_vget

macOS 10.6+

``` source
int (*vfs_vget)(struct mount *mp, ino64_t ino, struct vnode **vpp, vfs_context_t context);
```

