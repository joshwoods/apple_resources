

- Kernel
- vfs
-  vfs_clearflags 

Function

# vfs_clearflags

Clear flags on a mount.

macOS 10.4+

``` source
void vfs_clearflags(mount_t mp, uint64_t flags);
```

## Parameters 

`mp`  

Mount whose flags to set.

`flags`  

Flags to deactivate. Must be in the bitwise "OR" of MNT_VISFLAGMASK and MNT_CMDFLAGS.

## Return Value

void.

## Discussion

Sets mount flags to the bitwise "AND" of their current value and the complement of the specified bits.

