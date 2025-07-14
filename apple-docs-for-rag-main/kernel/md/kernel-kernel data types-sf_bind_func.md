

- Kernel
- Kernel Data Types
-  sf_bind_func 

Type Alias

# sf_bind_func

macOS 10.4+

``` source
typedef errno_t (*sf_bind_func)(void *cookie, socket_t so, const struct sockaddr *to);
```

## Parameters 

`cookie`  

Cookie value specified when the filter attach was called.

`so`  

The socket the filter is attached to.

`to`  

The local address of the socket will be bound to.

## Return Value

Return: 0 - The caller will continue with normal processing of the bind. EJUSTRETURN - The caller will return with a value of 0 (no error) from that point without further processing the bind command. The protocol layer will not see the call. Anything Else - The caller will rejecting the bind.

## Discussion

sf_bind_func is called before performing a bind operation on a socket.

