

- Kernel
- Deprecated Symbols
-  mbuf_mclget Deprecated

Function

# mbuf_mclget

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_mclget(mbuf_how_t how, mbuf_type_t type, mbuf_t *mbuf);
```

## Parameters 

`how`  

Blocking or non-blocking.

`type`  

The type of the mbuf.

`mbuf`  

The mbuf the cluster will be attached to.

## Return Value

0 on success, errno error on failure. If you specified NULL for the mbuf, any intermediate mbuf that may have been allocated will be freed. If you specify an mbuf value in \*mbuf, mbuf_mclget will not free it.

## Discussion

Allocate a cluster and attach it to an mbuf for use as external data. If mbuf points to a NULL mbuf_t, an mbuf will be allocated for you. If mbuf points to a non-NULL mbuf_t, mbuf_mclget may return a different mbuf_t than the one you passed in.

