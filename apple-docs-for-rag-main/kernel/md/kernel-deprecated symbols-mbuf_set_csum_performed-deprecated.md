

- Kernel
- Deprecated Symbols
-  mbuf_set_csum_performed Deprecated

Function

# mbuf_set_csum_performed

macOS 10.4–10.15.4Deprecated

``` source
errno_t mbuf_set_csum_performed(mbuf_t mbuf, mbuf_csum_performed_flags_t flags, u_int32_t value);
```

## Parameters 

`mbuf`  

The mbuf containing the packet.

`flags`  

Flags indicating which hardware checksum operations were performed.

`value`  

If the MBUF_CSUM_DID_DATA flag is set, value should be set to the value of the TCP or UDP header as calculated by the hardware.

## Return Value

0 upon success otherwise the errno error.

## Discussion

This is used by the driver to indicate to the stack which checksum operations were performed in hardware.

