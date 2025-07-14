

- Kernel
- Kernel Enumerations
- Anonymous
-  MBUF_CSUM_PSEUDO_HDR 

Enumeration Case

# MBUF_CSUM_PSEUDO_HDR

macOS 10.12+

``` source
MBUF_CSUM_PSEUDO_HDR = 0x0800
```

## Discussion

If set, this indicates that the checksum value for MBUF_CSUM_DID_DATA includes the pseudo header value. If this is not set, the stack will calculate the pseudo header value and add that to the checksum. The value of this bit is only valid when MBUF_CSUM_DID_DATA is set.

