

- NetworkingDriverKit
- IOUserNetworkEthernet
-  SetTxPacketHeadroom 

Instance Method

# SetTxPacketHeadroom

Reserves the specified number of bytes at the front of each packet.

DriverKit

``` source
kern_return_t SetTxPacketHeadroom(uint16_t numBytes);
```

## Parameters 

`numBytes`  

The number of bytes to reserve at the front of the packet buffer.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## See Also

### Configuring Link Attributes

SetTxPacketTailroom

Reserves the specified number of bytes at the end of each packet.

SetSoftwareVlanSupport

Enables software VLAN support.

SetMulticastAddresses

Sets the device addresses to use for multicast filtering.

SetAllMulticastModeEnable

Enables or disables multicast support for your service.

SetPromiscuousModeEnable

Enables or disables support for monitoriong all network packets.

SetWakeOnMagicPacketSupport

Tells the system whether the device supports being woken up when a specially formatted packet arrives.

SetWakeOnMagicPacketEnable

Enables or disables support for waking up the device when a specially formatted packet arrives.

IOUserNetworkMACAddress

A hardware address for a device.

