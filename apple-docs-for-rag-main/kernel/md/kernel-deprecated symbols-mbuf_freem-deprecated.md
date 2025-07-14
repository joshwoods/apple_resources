

- Kernel
- Deprecated Symbols
-  mbuf_freem Deprecated

Function

# mbuf_freem

macOS 10.4–10.15.4Deprecated

``` source
void mbuf_freem(mbuf_t mbuf);
```

## Parameters 

`mbuf`  

The first mbuf in the chain to free.

## Discussion

Frees a chain of mbufs link through mnext.

