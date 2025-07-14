

- Kernel
- Kernel Data Types
- vfsops
-  vfs_quotactl 

Instance Property

# vfs_quotactl

macOS 10.6+

``` source
int (*vfs_quotactl)(struct mount *mp, int cmds, uid_t uid, caddr_t arg, vfs_context_t context);
```

