

- Kernel
- vfs
-  vfs_iterate 

Function

# vfs_iterate

Iterate over all mountpoints with a callback. Used, for example, by sync().

macOS 10.4+

``` source
int vfs_iterate(int flags, int (*callout)(struct mount *, void *), void *arg);
```

## Parameters 

`flags`  

Unused.

`callback`  

Function which takes a mount and arbitrary passed-in "arg," and returns one of VFS_RETURNED_DONE or VFS_CLAIMED_DONE: end iteration and return success. VFS_RETURNED or VFS_CLAIMED: continue iterating. Anything else: continue iterating.

`arg`  

Arbitrary data to pass to callback.

## Return Value

0 for success, else an error code.

