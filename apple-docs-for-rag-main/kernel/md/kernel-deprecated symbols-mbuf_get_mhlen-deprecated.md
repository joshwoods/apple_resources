

- Kernel
- Deprecated Symbols
-  mbuf_get_mhlen Deprecated

Function

# mbuf_get_mhlen

macOS 10.4–10.15.4Deprecated

``` source
u_int32_t mbuf_get_mhlen(void);
```

## Return Value

The number of bytes of available data.

## Discussion

This routine returns the number of data bytes in a packet header mbuf. This is equivalent to the legacy MHLEN macro.

