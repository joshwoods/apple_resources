

- Kernel
- Deprecated Symbols
-  mbuf_pullup Deprecated

Function

# mbuf_pullup

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_pullup(mbuf_t *mbuf, size_t len);
```

## Parameters 

`mbuf`  

The mbuf in the chain the data should be contiguous in.

`len`  

The number of bytes to pull from the next mbuf(s).

## Return Value

0 upon success otherwise the errno error. In the case of an error, the mbuf chain has been freed.

## Discussion

Move the next len bytes in to mbuf from other mbufs in the chain. This is commonly used to get the IP and TCP or UDP header contiguous in the first mbuf. If mbuf_pullup fails, the entire mbuf chain will be freed.

