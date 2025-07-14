

- Kernel
- Deprecated Symbols
-  mbuf_gethdr Deprecated

Function

# mbuf_gethdr

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_gethdr(mbuf_how_t how, mbuf_type_t type, mbuf_t *mbuf);
```

## Parameters 

`how`  

Blocking or non-blocking.

`type`  

The type of the mbuf.

`mbuf`  

The mbuf.

## Return Value

0 on success, errno error on failure.

## Discussion

Allocates an mbuf without a cluster for external data. Sets a flag to indicate there is a packet header and initializes the packet header.

