

- Kernel
- Deprecated Symbols
-  mbuf_pkthdr_setrcvif Deprecated

Function

# mbuf_pkthdr_setrcvif

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_pkthdr_setrcvif(mbuf_t mbuf, ifnet_t ifp);
```

## Parameters 

`mbuf`  

The mbuf containing the packet header.

`ifnet`  

A reference to an interface.

## Return Value

0 upon success otherwise the errno error.

## Discussion

Sets the interface the packet was received on.

