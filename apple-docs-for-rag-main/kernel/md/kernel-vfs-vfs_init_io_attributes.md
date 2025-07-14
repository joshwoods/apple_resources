

- Kernel
- vfs
-  vfs_init_io_attributes 

Function

# vfs_init_io_attributes

Set I/O attributes on a mountpoint based on device properties.

macOS 10.6+

``` source
int vfs_init_io_attributes(vnode_t devvp, mount_t mp);
```

## Parameters 

`devvp`  

Block device vnode from which a filesystem is being mounted.

`mp`  

Mountpoint whose I/O parameters to initialize.

## Return Value

0 for success, else an error code.

