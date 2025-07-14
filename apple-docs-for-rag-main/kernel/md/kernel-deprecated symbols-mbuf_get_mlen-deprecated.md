

- Kernel
- Deprecated Symbols
-  mbuf_get_mlen Deprecated

Function

# mbuf_get_mlen

macOS 10.4–10.15.4Deprecated

``` source
u_int32_t mbuf_get_mlen(void);
```

## Return Value

The number of bytes of available data.

## Discussion

This routine returns the number of data bytes in a normal mbuf, i.e. an mbuf that is not a packet header, nor one with an external cluster attached to it. This is equivalent to the legacy MLEN macro.

