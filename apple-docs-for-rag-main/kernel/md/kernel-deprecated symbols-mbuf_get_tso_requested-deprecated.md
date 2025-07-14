

- Kernel
- Deprecated Symbols
-  mbuf_get_tso_requested Deprecated

Function

# mbuf_get_tso_requested

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_get_tso_requested(mbuf_t mbuf, mbuf_tso_request_flags_t *request, u_int32_t *mss);
```

## Parameters 

`mbuf`  

The mbuf containing the packet.

`request`  

Flags indicating which values are being requested for this packet.

`value`  

The requested value.

## Return Value

0 upon success otherwise the errno error.

## Discussion

This function is used by the driver to determine which checksum operations should be performed in hardware.

