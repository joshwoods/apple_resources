

- Kernel
- Deprecated Symbols
-  mbuf_clear_csum_requested Deprecated

Function

# mbuf_clear_csum_requested

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_clear_csum_requested(mbuf_t mbuf);
```

## Parameters 

`mbuf`  

The mbuf containing the packet.

## Return Value

0 upon success otherwise the errno error.

## Discussion

This function clears the checksum request flags.

