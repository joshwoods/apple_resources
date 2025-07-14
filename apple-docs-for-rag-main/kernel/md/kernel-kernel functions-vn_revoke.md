

- Kernel
- Kernel Functions
-  vn_revoke 

Function

# vn_revoke

Invalidate all references to a vnode.

macOS 10.4+

``` source
int vn_revoke(vnode_t vp, int flags, vfs_context_t ctx);
```

## Parameters 

`vp`  

The vnode to revoke.

`flags`  

Unused.

`ctx`  

Context against which to validate operation.

## Return Value

0 always.

## Discussion

Reclaims the vnode, giving it deadfs vnops (though not halting operations which are already in progress). Also reclaims all aliased vnodes (important for devices). People holding usecounts on the vnode, e.g. processes with the file open, will find that all subsequent operations but closing the file fail.

