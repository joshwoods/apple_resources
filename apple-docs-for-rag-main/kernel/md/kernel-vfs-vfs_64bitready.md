

- Kernel
- vfs
-  vfs_64bitready 

Function

# vfs_64bitready

Check if the filesystem associated with a mountpoint is marked ready for interaction with 64-bit user processes.

macOS 10.4+

``` source
int vfs_64bitready(mount_t mp);
```

## Parameters 

`mp`  

Mount to test.

## Return Value

Nonzero if filesystem is ready for 64-bit; 0 otherwise.

