

- Kernel
- vfs
-  vfs_unbusy 

Function

# vfs_unbusy

"Unbusy" a mountpoint by releasing its read-write lock.

macOS 10.4+

``` source
void vfs_unbusy(mount_t mp);
```

## Parameters 

`mp`  

Mount to unbusy.

## Return Value

void.

## Discussion

A successful vfs_busy() must be followed by a vfs_unbusy() to release the lock on the mount.

