

- Kernel
- vfs
-  vfs_context_ucred 

Function

# vfs_context_ucred

Get the credential associated with a vfs_context_t.

macOS 10.4+

``` source
kauth_cred_t vfs_context_ucred(vfs_context_t ctx);
```

## Parameters 

`ctx`  

Context whose associated process to find.

## Return Value

Process if available, NULL otherwise.

## Discussion

Succeeds if and only if the context has a thread, the thread has a task, and the task has a BSD proc.

