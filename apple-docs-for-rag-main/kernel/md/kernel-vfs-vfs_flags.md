

- Kernel
- vfs
-  vfs_flags 

Function

# vfs_flags

Retrieve mount flags.

macOS 10.4+

``` source
uint64_t vfs_flags(mount_t mp);
```

## Parameters 

`mp`  

Mount whose flags to grab.

## Return Value

Flags.

## Discussion

Results will be in the bitwise "OR" of MNT_VISFLAGMASK and MNT_CMDFLAGS.

