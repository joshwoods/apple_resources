

- Kernel
- Deprecated Symbols
-  mbuf_get_minclsize Deprecated

Function

# mbuf_get_minclsize

macOS 10.4–10.15.4Deprecated

``` source
u_int32_t mbuf_get_minclsize(void);
```

## Return Value

The minimum number of bytes before a cluster will be used.

## Discussion

This routine returns the minimum number of data bytes before an external cluster is used. This is equivalent to the legacy MINCLSIZE macro.

