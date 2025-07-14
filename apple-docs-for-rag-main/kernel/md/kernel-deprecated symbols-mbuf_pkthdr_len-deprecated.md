

- Kernel
- Deprecated Symbols
-  mbuf_pkthdr_len Deprecated

Function

# mbuf_pkthdr_len

macOS 10.4–10.15.4Deprecated

``` source
size_t mbuf_pkthdr_len(const mbuf_t mbuf);
```

## Parameters 

`mbuf`  

The mbuf containing the packet header with the length to be changed.

## Return Value

The length, in bytes, of the packet.

## Discussion

Returns the length as reported by the packet header.

