

- Kernel
- Deprecated Symbols
-  mbuf_pkthdr_adjustlen Deprecated

Function

# mbuf_pkthdr_adjustlen

macOS 10.4–10.15.4Deprecated

``` source
void mbuf_pkthdr_adjustlen(mbuf_t mbuf, int amount);
```

## Parameters 

`mbuf`  

The mbuf containing the packet header.

`amount`  

The number of bytes to adjust the packet header length field by.

## Discussion

Adjusts the length of the packet in the packet header.

