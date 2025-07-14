

- Kernel
- Deprecated Symbols
-  mbuf_copydata Deprecated

Function

# mbuf_copydata

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_copydata(const mbuf_t mbuf, size_t offset, size_t length, void *out_data);
```

## Parameters 

`mbuf`  

The mbuf chain to copy data out of.

`offset`  

The offset in to the mbuf to start copying.

`length`  

The number of bytes to copy.

`out_data`  

A pointer to the location where the data will be copied.

## Return Value

0 upon success otherwise the errno error.

## Discussion

Copies data out of an mbuf in to a specified buffer. If the data is stored in a chain of mbufs, the data will be copied from each mbuf in the chain until length bytes have been copied.

