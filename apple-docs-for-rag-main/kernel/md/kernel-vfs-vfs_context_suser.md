

- Kernel
- vfs
-  vfs_context_suser 

Function

# vfs_context_suser

Determine if a vfs_context_t corresponds to the superuser.

macOS 10.4+

``` source
int vfs_context_suser(vfs_context_t ctx);
```

## Parameters 

`ctx`  

Context to examine.

## Return Value

Nonzero if context belongs to superuser, 0 otherwise.

