

- Kernel
- vfs
-  vfs_setmaxsymlen 

Function

# vfs_setmaxsymlen

Set the maximum length of a symbolic link on a filesystem.

macOS 10.4+

``` source
void vfs_setmaxsymlen(mount_t mp, uint32_t symlen);
```

## Parameters 

`mp`  

Mount on which to set symlink length cap.

`symlen`  

Length to set.

## Return Value

Max symlink length.

