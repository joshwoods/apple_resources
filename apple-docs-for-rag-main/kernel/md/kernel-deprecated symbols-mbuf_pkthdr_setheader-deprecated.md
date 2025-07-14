

- Kernel
- Deprecated Symbols
-  mbuf_pkthdr_setheader Deprecated

Function

# mbuf_pkthdr_setheader

macOS 10.4–10.15.4Deprecated

``` source
void mbuf_pkthdr_setheader(mbuf_t mbuf, void *header);
```

## Parameters 

`mbuf`  

The mbuf containing the packet header.

`ifnet`  

A pointer to the header.

## Return Value

0 upon success otherwise the errno error.

## Discussion

Sets the pointer to the packet header.

