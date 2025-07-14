

- Kernel
- Kernel Data Types
- vfsops
-  vfs_ioctl 

Instance Property

# vfs_ioctl

macOS 10.12+

``` source
int (*vfs_ioctl)(struct mount *mp, u_long command, caddr_t data, int flags, vfs_context_t context);
```

