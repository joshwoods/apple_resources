

- Kernel
- Deprecated Symbols
-  mbuf_setflags Deprecated

Function

# mbuf_setflags

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_setflags(mbuf_t mbuf, mbuf_flags_t flags);
```

## Parameters 

`mbuf`  

The mbuf.

`flags`  

The flags that should be set, all other flags will be cleared. Certain flags such as MBUF_EXT cannot be altered.

## Return Value

0 upon success otherwise the errno error.

## Discussion

Sets the set of set flags.

