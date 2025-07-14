

- Kernel
- Deprecated Symbols
-  mbuf_pulldown Deprecated

Function

# mbuf_pulldown

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_pulldown(mbuf_t src, size_t *offset, size_t length, mbuf_t *location);
```

## Parameters 

`src`  

The start of the mbuf chain.

`offset`  

Pass in a pointer to a value with the offset of the data you're interested in making contiguous. Upon success, this will be overwritten with the offset from the mbuf returned in location.

`length`  

The length of data that should be made contiguous.

`location`  

Upon success, \*location will be the mbuf the data is in.

## Return Value

0 upon success otherwise the errno error.

## Discussion

Make length bytes at offset in the mbuf chain contiguous. Nothing before offset bytes in the chain will be modified. Upon return, location will be the mbuf the data is contiguous in and offset will be the offset in that mbuf at which the data is located. In the case of a failure, the mbuf chain will be freed.

