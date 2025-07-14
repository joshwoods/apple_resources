

- Kernel
- vfs
-  vfs_context_proc 

Function

# vfs_context_proc

Get the BSD process structure associated with a vfs_context_t.

macOS 10.4+

``` source
proc_t vfs_context_proc(vfs_context_t ctx);
```

## Parameters 

`ctx`  

Context whose associated process to find.

## Return Value

Process if available, NULL otherwise.

