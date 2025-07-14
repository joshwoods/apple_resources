

- Kernel
- Deprecated Symbols
-  mbuf_adj Deprecated

Function

# mbuf_adj

macOS 10.4–10.15.4Deprecated

``` source
void mbuf_adj(mbuf_t mbuf, int len);
```

## Parameters 

`mbuf`  

The mbuf chain to trim.

`len`  

The number of bytes to trim from the mbuf chain.

## Discussion

Trims len bytes from the mbuf. If the length is greater than zero, the bytes are trimmed from the front of the mbuf. If the length is less than zero, the bytes are trimmed from the end of the mbuf chain.

