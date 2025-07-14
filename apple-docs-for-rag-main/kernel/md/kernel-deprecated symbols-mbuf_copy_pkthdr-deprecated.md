

- Kernel
- Deprecated Symbols
-  mbuf_copy_pkthdr Deprecated

Function

# mbuf_copy_pkthdr

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_copy_pkthdr(mbuf_t dest, const mbuf_t src);
```

## Parameters 

`src`  

The mbuf from which the packet header will be copied.

`mbuf`  

The mbuf to which the packet header will be copied.

## Return Value

0 upon success otherwise the errno error.

## Discussion

Copies the packet header from src to dest.

