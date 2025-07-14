

- Kernel
- vfs
-  vfs_context_current 

Function

# vfs_context_current

Get the vfs_context for the current thread, or the kernel context if there is no context for current thread.

macOS 10.5+

``` source
vfs_context_t vfs_context_current(void);
```

## Return Value

Context for current thread, or kernel context if thread context is unavailable.

## Discussion

Kexts should not use this function--it is preferred to use vfs_context_create(NULL) and vfs_context_rele(), which ensure proper reference counting of underlying structures.

