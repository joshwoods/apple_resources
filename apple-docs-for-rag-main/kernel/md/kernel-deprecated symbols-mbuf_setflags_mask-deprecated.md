

- Kernel
- Deprecated Symbols
-  mbuf_setflags_mask Deprecated

Function

# mbuf_setflags_mask

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_setflags_mask(mbuf_t mbuf, mbuf_flags_t flags, mbuf_flags_t mask);
```

## Parameters 

`mbuf`  

The mbuf.

`flags`  

The flags that should be set or cleared. Certain flags such as MBUF_EXT cannot be altered.

`mask`  

The mask controlling which flags will be modified.

## Return Value

0 upon success otherwise the errno error.

## Discussion

Useful for setting or clearing individual flags. Easier than calling mbuf_setflags(m, mbuf_flags(m) \| M_FLAG).

