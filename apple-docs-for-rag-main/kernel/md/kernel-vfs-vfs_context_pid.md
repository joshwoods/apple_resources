

- Kernel
- vfs
-  vfs_context_pid 

Function

# vfs_context_pid

Get the process id of the BSD process associated with a vfs_context_t.

macOS 10.4+

``` source
int vfs_context_pid(vfs_context_t ctx);
```

## Parameters 

`ctx`  

Context whose associated process to find.

## Return Value

Process id.

