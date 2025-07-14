

- Kernel
- vfs
-  vflush 

Function

# vflush

Reclaim the vnodes for a mount.

macOS 10.4+

``` source
int vflush(struct mount *mp, struct vnode *skipvp, int flags);
```

## Parameters 

`mp`  

The mount with the vnodes to terminate.

`skipvp`  

A specific vnode to not reclaim or to let interrupt an unforced flush.

`flags`  

Controls that indicate how to handle vnodes.

## Return Value

0 for success, EBUSY if vnodes were busy and FORCECLOSE was not set.

## Discussion

This function is used to clear out the vnodes associated with a mount as part of the unmount process. Its parameters can determine which vnodes to skip in the process and whether in-use vnodes should be forcibly reclaimed. File systems should call this function from their unmount code, because VFS code will always call it with SKIPROOT \| SKIPSWAP \| SKIPSYSTEM; file systems must take care of such vnodes themselves.

