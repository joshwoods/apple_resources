

- Kernel
- Kernel Functions
-  sflt_register Deprecated

Function

# sflt_register

macOS 10.4–10.15Deprecated

``` source
errno_t sflt_register(const struct sflt_filter *filter, int domain, int type, int protocol);
```

## Parameters 

`filter`  

A structure describing the filter.

`domain`  

The protocol domain these filters will be attached to.

`type`  

The socket type these filters will be attached to.

`protocol`  

The protocol these filters will be attached to.

## Return Value

0 on success otherwise the errno error.

## Discussion

Registers a socket filter. See 'man 2 socket' for a desciption of domain, type, and protocol.

