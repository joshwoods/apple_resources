

- Kernel
- vfs
-  vfs_context_create 

Function

# vfs_context_create

Create a new vfs_context_t with appropriate references held.

macOS 10.4+

``` source
vfs_context_t vfs_context_create(vfs_context_t ctx);
```

## Parameters 

`ctx`  

Context to copy, or NULL to use information from running thread.

## Return Value

The new context, or NULL in the event of failure.

## Discussion

The context must be released with vfs_context_rele() when no longer in use.

