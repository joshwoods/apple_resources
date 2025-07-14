

- Kernel
- vfs
-  vfs_typenum 

Function

# vfs_typenum

Get (archaic) filesystem type number.

macOS 10.4+

``` source
int vfs_typenum(mount_t mp);
```

## Parameters 

`mp`  

Mount for which to get type number.

## Return Value

Type number.

## Discussion

Filesystem type numbers are an old construct; most filesystems just get a number assigned based on the order in which they are registered with the system.

