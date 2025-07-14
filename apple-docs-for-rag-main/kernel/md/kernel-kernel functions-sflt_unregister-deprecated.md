

- Kernel
- Kernel Functions
-  sflt_unregister Deprecated

Function

# sflt_unregister

macOS 10.4–10.15Deprecated

``` source
errno_t sflt_unregister(sflt_handle handle);
```

## Parameters 

`handle`  

The sf_handle of the socket filter to unregister.

## Return Value

0 on success otherwise the errno error.

## Discussion

Unregisters a socket filter. This will not detach the socket filter from all sockets it may be attached to at the time, it will just prevent the socket filter from being attached to any new sockets.

