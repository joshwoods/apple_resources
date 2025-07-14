

- Kernel
- Deprecated Symbols
-  mbuf_split Deprecated

Function

# mbuf_split

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_split(mbuf_t src, size_t offset, mbuf_how_t how, mbuf_t *new_mbuf);
```

## Parameters 

`src`  

The mbuf to be split.

`offset`  

The offset in the buffer where the mbuf should be split.

`how`  

Blocking or non-blocking.

`new_mbuf`  

Upon success, the second half of the split mbuf chain.

## Return Value

0 upon success otherwise the errno error. In the case of failure, the original mbuf chain passed in to src will be preserved.

## Discussion

Split an mbuf chain at a specific offset.

