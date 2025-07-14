

- Kernel
- vfs
-  vfs_context_issignal 

Function

# vfs_context_issignal

Get a bitfield of pending signals for the BSD process associated with a vfs_context_t.

macOS 10.4+

``` source
int vfs_context_issignal(vfs_context_t ctx, sigset_t mask);
```

## Parameters 

`ctx`  

Context whose associated process to find.

## Return Value

Bitfield of pending signals.

## Discussion

The bitfield is constructed using the sigmask() macro, in the sense of bits \|= sigmask(SIGSEGV).

