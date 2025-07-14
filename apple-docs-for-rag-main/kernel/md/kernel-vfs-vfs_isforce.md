

- Kernel
- vfs
-  vfs_isforce 

Function

# vfs_isforce

Determine if a forced unmount is in progress.

macOS 10.4+

``` source
int vfs_isforce(mount_t mp);
```

## Parameters 

`mp`  

Mount to test.

## Return Value

Nonzero if a request has been made to forcibly unmount, else 0.

## Discussion

A forced unmount invalidates open files.

