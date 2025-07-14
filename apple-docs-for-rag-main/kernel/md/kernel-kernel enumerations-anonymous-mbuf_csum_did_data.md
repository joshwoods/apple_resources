

- Kernel
- Kernel Enumerations
- Anonymous
-  MBUF_CSUM_DID_DATA 

Enumeration Case

# MBUF_CSUM_DID_DATA

macOS 10.12+

``` source
MBUF_CSUM_DID_DATA = 0x0400
```

## Discussion

Indicates that the TCP or UDP checksum was calculated. The value for the checksum calculated in hardware should be passed as the second parameter of mbuf_set_csum_performed. The hardware calculated checksum value can be retrieved using the second parameter passed to mbuf_get_csum_performed. This should be done for IPv4 or IPv6.

