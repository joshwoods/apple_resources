

- Kernel
- vfs
-  vfs_maxsymlen 

Function

# vfs_maxsymlen

Get the maximum length of a symbolic link on a filesystem.

macOS 10.4+

``` source
uint32_t vfs_maxsymlen(mount_t mp);
```

## Parameters 

`mp`  

Mount from which to get symlink length cap.

## Return Value

Max symlink length.

