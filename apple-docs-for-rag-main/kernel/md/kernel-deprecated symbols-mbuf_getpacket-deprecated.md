

- Kernel
- Deprecated Symbols
-  mbuf_getpacket Deprecated

Function

# mbuf_getpacket

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_getpacket(mbuf_how_t how, mbuf_t *mbuf);
```

## Parameters 

`how`  

Blocking or non-blocking.

`mbuf`  

Upon success, \*mbuf will be a reference to the new mbuf.

## Return Value

0 on success, errno error on failure.

## Discussion

Allocate an mbuf, allocate and attach a cluster, and set the packet header flag.

