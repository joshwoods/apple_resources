

- Kernel
- Deprecated Symbols
-  mbuf_align_32 Deprecated

Function

# mbuf_align_32

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_align_32(mbuf_t mbuf, size_t len);
```

## Parameters 

`mbuf`  

The mbuf.

`len`  

The minimum length of space that should follow the new data location.

## Return Value

0 on success, errno error on failure.

## Discussion

mbuf_align_32 is a replacement for M_ALIGN and MH_ALIGN. mbuf_align_32 will set the data pointer to a location aligned on a four byte boundry with at least 'len' bytes between the data pointer and the end of the data block.

