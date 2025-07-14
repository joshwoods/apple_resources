

- Kernel
- Deprecated Symbols
-  mbuf_setlen Deprecated

Function

# mbuf_setlen

macOS 10.4–10.15.4Deprecated

``` source
void mbuf_setlen(mbuf_t mbuf, size_t len);
```

## Parameters 

`mbuf`  

The mbuf.

`len`  

The new length.

## Return Value

0 upon success otherwise the errno error.

## Discussion

Sets the length of data in this packet. Be careful to not set the length over the space available in the mbuf.

