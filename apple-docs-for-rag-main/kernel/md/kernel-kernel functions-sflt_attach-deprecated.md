

- Kernel
- Kernel Functions
-  sflt_attach Deprecated

Function

# sflt_attach

macOS 10.4–10.15Deprecated

``` source
errno_t sflt_attach(socket_t socket, sflt_handle handle);
```

## Parameters 

`socket`  

The socket the filter should be attached to.

`handle`  

The handle of the registered filter to be attached.

## Return Value

0 on success otherwise the errno error.

## Discussion

Attaches a socket filter to the specified socket. A filter must be registered before it can be attached.

