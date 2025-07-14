

- Kernel
- Deprecated Symbols
-  IOExitThread Deprecated

Function

# IOExitThread

Deprecated function - use thread_terminate(). Terminate execution of current thread.

macOS 10.0–10.6Deprecated

``` source
void IOExitThread(void);
```

## Discussion

This function destroys the currently running thread, and does not return.

