

- Kernel
- Deprecated Symbols
-  mbuf_prepend Deprecated

Function

# mbuf_prepend

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_prepend(mbuf_t *mbuf, size_t len, mbuf_how_t how);
```

## Parameters 

`mbuf`  

The mbuf to prepend data to. This may change if a new mbuf must be allocated or may be NULL if the operation fails.

`len`  

The length, in bytes, to be prepended to the mbuf.

`how`  

Blocking or non-blocking.

## Return Value

0 upon success otherwise the errno error.

## Discussion

Prepend len bytes to an mbuf. If there is space (mbuf_leadingspace \>= len), the mbuf's data ptr is changed and the same mbuf is returned. If there is no space, a new mbuf may be allocated and prepended to the mbuf chain. If the operation fails, the mbuf may be freed (\*mbuf will be NULL).

