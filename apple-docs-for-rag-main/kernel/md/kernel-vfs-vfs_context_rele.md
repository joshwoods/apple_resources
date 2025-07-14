

- Kernel
- vfs
-  vfs_context_rele 

Function

# vfs_context_rele

Release references on components of a context and deallocate it.

macOS 10.4+

``` source
int vfs_context_rele(vfs_context_t ctx);
```

## Parameters 

`ctx`  

Context to release.

## Return Value

Always 0.

## Discussion

A context should not be referenced after vfs_context_rele has been called.

