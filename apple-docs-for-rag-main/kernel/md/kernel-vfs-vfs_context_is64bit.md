

- Kernel
- vfs
-  vfs_context_is64bit 

Function

# vfs_context_is64bit

Determine if a vfs_context_t corresponds to a 64-bit user process.

macOS 10.4+

``` source
int vfs_context_is64bit(vfs_context_t ctx);
```

## Parameters 

`ctx`  

Context to examine.

## Return Value

Nonzero if context is of 64-bit process, 0 otherwise.

