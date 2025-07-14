

- Kernel
- Deprecated Symbols
-  mbuf_pkthdr_setlen Deprecated

Function

# mbuf_pkthdr_setlen

macOS 10.4–10.15.4Deprecated

``` source
void mbuf_pkthdr_setlen(mbuf_t mbuf, size_t len);
```

## Parameters 

`mbuf`  

The mbuf containing the packet header.

`len`  

The new length of the packet.

## Discussion

Sets the length of the packet in the packet header.

