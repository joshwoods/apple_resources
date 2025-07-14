

- Kernel
- Deprecated Symbols
-  mbuf_setnext Deprecated

Function

# mbuf_setnext

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_setnext(mbuf_t mbuf, mbuf_t next);
```

## Parameters 

`mbuf`  

The mbuf.

`next`  

The new next mbuf.

## Return Value

0 upon success otherwise the errno error.

## Discussion

Sets the next mbuf in the chain.

