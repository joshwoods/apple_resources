

- Kernel
- Kernel Functions
-  sflt_detach Deprecated

Function

# sflt_detach

macOS 10.4–10.15Deprecated

``` source
errno_t sflt_detach(socket_t socket, sflt_handle handle);
```

## Parameters 

`socket`  

The socket the filter should be detached from.

`handle`  

The handle of the registered filter to be detached.

## Return Value

0 on success otherwise the errno error.

## Discussion

Detaches a socket filter from a specified socket.

