

- Kernel
- Deprecated Symbols
-  mbuf_dup Deprecated

Function

# mbuf_dup

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_dup(const mbuf_t src, mbuf_how_t how, mbuf_t *new_mbuf);
```

## Parameters 

`src`  

The source mbuf.

`how`  

Blocking or non-blocking.

`new_mbuf`  

Upon success, the newly allocated mbuf.

## Return Value

0 upon success otherwise the errno error.

## Discussion

Exactly duplicates an mbuf chain. If the original mbuf contains a packet header (including tags), the new mbuf will have the same packet header contents and a copy of each tag associated with the original mbuf.

