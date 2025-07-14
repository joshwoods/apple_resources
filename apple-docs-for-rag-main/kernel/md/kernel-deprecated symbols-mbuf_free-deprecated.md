

- Kernel
- Deprecated Symbols
-  mbuf_free Deprecated

Function

# mbuf_free

macOS 10.4–10.15.4Deprecated

``` source
mbuf_t mbuf_free(mbuf_t mbuf);
```

## Parameters 

`mbuf`  

The mbuf to free.

## Return Value

The next mbuf in the chain.

## Discussion

Frees a single mbuf. Not commonly used because it doesn't touch the rest of the mbufs on the chain.

