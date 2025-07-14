

- Kernel
- vfs
-  vfs_unmountbyfsid 

Function

# vfs_unmountbyfsid

Find a filesystem by ID and unmount it.

macOS 10.5+

``` source
int vfs_unmountbyfsid(fsid_t *fsid, int flags, vfs_context_t ctx);
```

## Parameters 

`fsid`  

ID of filesystem to unmount, as found through (for example) statfs.

`flags`  

MNT_FORCE: forcibly invalidate files open on the mount (though in-flight I/O operations will be allowed to complete).

`ctx`  

Context against which to authenticate unmount operation.

## Return Value

0 for succcess, nonero for failure.

