

- Kernel
- Deprecated Symbols
-  mbuf_clear_csum_performed Deprecated

Function

# mbuf_clear_csum_performed

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_clear_csum_performed(mbuf_t mbuf);
```

## Parameters 

`mbuf`  

The mbuf containing the packet.

## Return Value

0 upon success otherwise the errno error.

## Discussion

Clears the hardware checksum flags and values.

