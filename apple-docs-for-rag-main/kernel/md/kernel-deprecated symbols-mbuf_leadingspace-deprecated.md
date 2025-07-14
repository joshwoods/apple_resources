

- Kernel
- Deprecated Symbols
-  mbuf_leadingspace Deprecated

Function

# mbuf_leadingspace

macOS 10.4–10.15.4Deprecated

``` source
size_t mbuf_leadingspace(const mbuf_t mbuf);
```

## Parameters 

`mbuf`  

The mbuf.

## Return Value

The number of unused bytes at the start of the mbuf.

## Discussion

Determines the space available in the mbuf proceeding the current data.

