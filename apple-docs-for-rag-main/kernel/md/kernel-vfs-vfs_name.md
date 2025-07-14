

- Kernel
- vfs
-  vfs_name 

Function

# vfs_name

Copy filesystem name into a buffer.

macOS 10.4+

``` source
void vfs_name(mount_t mp, char *buffer);
```

## Parameters 

`mp`  

Mount for which to get name.

`buffer`  

Destination for name; length should be at least MFSNAMELEN.

## Return Value

void.

## Discussion

Get filesystem name; this refers to the filesystem type of which a mount is an instantiation, rather than a name specific to the mountpoint.

