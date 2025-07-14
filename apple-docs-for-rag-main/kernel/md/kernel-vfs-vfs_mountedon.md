

- Kernel
- vfs
-  vfs_mountedon 

Function

# vfs_mountedon

Check whether a given block device has a filesystem mounted on it.

macOS 10.4+

``` source
int vfs_mountedon(struct vnode *vp);
```

## Parameters 

`vp`  

The vnode to test.

## Return Value

EBUSY if vnode is indeed the source of a filesystem; 0 if it is not.

## Discussion

Note that this is NOT a check for a covered vnode (the directory upon which a filesystem is mounted)--it is a test for whether a block device is being used as the source of a filesystem. Note that a block device marked as being mounted on cannot be opened.

