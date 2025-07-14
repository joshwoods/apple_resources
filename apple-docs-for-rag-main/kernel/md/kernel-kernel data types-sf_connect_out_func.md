

- Kernel
- Kernel Data Types
-  sf_connect_out_func 

Type Alias

# sf_connect_out_func

macOS 10.4+

``` source
typedef errno_t (*sf_connect_out_func)(void *cookie, socket_t so, const struct sockaddr *to);
```

## Parameters 

`cookie`  

Cookie value specified when the filter attach was called.

`so`  

The socket the filter is attached to.

`to`  

The remote address of the outbound connection.

## Return Value

Return: 0 - The caller will continue with normal processing of the connection. EJUSTRETURN - The caller will return with a value of 0 (no error) from that point without further processing the connect command. The protocol layer will not see the call. Anything Else - The caller will rejecting the outbound connection.

## Discussion

sf_connect_out_func is called to filter outbound connections. A protocol will call this before initiating an outbound connection.

