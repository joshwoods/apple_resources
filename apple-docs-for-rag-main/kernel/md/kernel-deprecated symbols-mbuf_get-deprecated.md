

- Kernel
- Deprecated Symbols
-  mbuf_get Deprecated

Function

# mbuf_get

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_get(mbuf_how_t how, mbuf_type_t type, mbuf_t *mbuf);
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

Allocates an mbuf without a cluster for external data.

