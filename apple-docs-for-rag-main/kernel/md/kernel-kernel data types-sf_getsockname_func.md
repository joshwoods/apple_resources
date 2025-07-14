

- Kernel
- Kernel Data Types
-  sf_getsockname_func 

Type Alias

# sf_getsockname_func

macOS 10.4+

``` source
typedef int (*sf_getsockname_func)(void *cookie, socket_t so, struct sockaddr **sa);
```

## Parameters 

`cookie`  

Cookie value specified when the filter attach was called.

`so`  

The socket the filter is attached to.

`sa`  

A pointer to a socket address pointer.

## Return Value

If you return a non-zero value, processing will stop. If you return EJUSTRETURN, no further filters will be called but a result of zero will be returned to the caller of getsockname.

## Discussion

sf_getsockname_func is called to allow a filter to to intercept the getsockname function. When called, sa will point to a pointer to a socket address that was malloced in zone M_SONAME. If you want to replace this address, either modify the currenty copy or allocate a new one and free the old one.

