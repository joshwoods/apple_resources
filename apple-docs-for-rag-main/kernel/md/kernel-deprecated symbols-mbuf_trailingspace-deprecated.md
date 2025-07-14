

- Kernel
- Deprecated Symbols
-  mbuf_trailingspace Deprecated

Function

# mbuf_trailingspace

macOS 10.4–10.15.4Deprecated

``` source
size_t mbuf_trailingspace(const mbuf_t mbuf);
```

## Parameters 

`mbuf`  

The mbuf.

## Return Value

The number of unused bytes following the current data.

## Discussion

Determines the space available in the mbuf following the current data.

