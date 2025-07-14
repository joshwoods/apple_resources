

- Kernel
- Deprecated Symbols
-  mbuf_datastart Deprecated

Function

# mbuf_datastart

macOS 10.4–10.15.4Deprecated

``` source
void * mbuf_datastart(mbuf_t mbuf);
```

## Parameters 

`mbuf`  

The mbuf.

## Return Value

A pointer to smallest possible value for data.

## Discussion

Returns the start of the space set aside for storing data in an mbuf. An mbuf's data may come from a cluster or be embedded in the mbuf structure itself. The data pointer retrieved by mbuf_data may not be at the start of the data (mbuf_leadingspace will be non-zero). This function will return a pointer that matches mbuf_data() - mbuf_leadingspace().

