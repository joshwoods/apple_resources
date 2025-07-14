

- Kernel
- sys
- vnop_clonefile_args
-  a_dir_clone_authorizer 

Instance Property

# a_dir_clone_authorizer

macOS 10.12.4+

``` source
int (*a_dir_clone_authorizer)(struct vnode_attr *vap, kauth_action_t action, struct vnode_attr *dvap, vnode_t sdvp, mount_t mp, dir_clone_authorizer_op_t vattr_op, uint32_t flags, vfs_context_t ctx, void *reserved);
```

