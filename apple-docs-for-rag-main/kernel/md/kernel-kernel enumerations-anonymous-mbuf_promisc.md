

- Kernel
- Kernel Enumerations
- Anonymous
-  MBUF_PROMISC 

Enumeration Case

# MBUF_PROMISC

macOS 10.12+

``` source
MBUF_PROMISC = 0x2000
```

## Discussion

Indicates this packet was only received because the interface is in promiscuous mode. This should be set by the demux function. These packets will be discarded after being passed to any interface filters.

