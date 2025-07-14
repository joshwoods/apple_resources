

- Kernel
- Kernel Enumerations
- Anonymous
-  kIOEthernetWakeOnPacketAddressMatch 

Enumeration Case

# kIOEthernetWakeOnPacketAddressMatch

macOS 10.12+

``` source
kIOEthernetWakeOnPacketAddressMatch = 0x00000002
```

## Discussion

Reception of a packet which passes through any of the address filtering mechanisms based on its destination Ethernet address. This may include unicast, broadcast, or multicast addresses depending on the current state and setting of the corresponding packet filters.

