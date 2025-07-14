

- Kernel
- Kernel Data Types
-  sf_detach_func 

Type Alias

# sf_detach_func

macOS 10.4+

``` source
typedef void (*sf_detach_func)(void *cookie, socket_t so);
```

## Parameters 

`cookie`  

Cookie value specified when the filter attach was called.

`so`  

The socket the filter is attached to.

## Return Value

If you return a non-zero value, your filter will not be attached to this socket.

## Discussion

sf_detach_func is called to notify the filter it has been detached from a socket. If the filter allocated any memory for this attachment, it should be freed. This function will be called when the socket is disposed of.

