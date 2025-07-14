

- Kernel
- vfs
-  vfs_setflags 

Function

# vfs_setflags

Set flags on a mount.

macOS 10.4+

``` source
void vfs_setflags(mount_t mp, uint64_t flags);
```

## Parameters 

`mp`  

Mount whose flags to set.

`flags`  

Flags to activate. Must be in the bitwise "OR" of MNT_VISFLAGMASK and MNT_CMDFLAGS.

## Return Value

Flags.

## Discussion

Sets mount flags to the bitwise "OR" of their current value and the specified bits. Often used by a filesystem as part of the mount process.

