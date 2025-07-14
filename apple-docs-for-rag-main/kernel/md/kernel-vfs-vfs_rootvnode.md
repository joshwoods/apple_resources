

- Kernel
- vfs
-  vfs_rootvnode 

Function

# vfs_rootvnode

Returns the root vnode with an iocount.

macOS 10.5+

``` source
vnode_t vfs_rootvnode(void);
```

## Return Value

Pointer to root vnode if successful; error code if there is a problem taking an iocount.

## Discussion

Caller must vnode_put() the root node when done.

