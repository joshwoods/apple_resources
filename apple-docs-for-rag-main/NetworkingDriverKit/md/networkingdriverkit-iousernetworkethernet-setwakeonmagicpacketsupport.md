

- NetworkingDriverKit
- IOUserNetworkEthernet
-  SetWakeOnMagicPacketSupport 

Instance Method

# SetWakeOnMagicPacketSupport

Tells the system whether the device supports being woken up when a specially formatted packet arrives.

DriverKit

``` source
kern_return_t SetWakeOnMagicPacketSupport(bool isSupported);
```

## Parameters 

`isSupported`  

If `YES`, the device supports waking up when the network receives a magic packet; otherwise, it doesn’t.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## See Also

### Configuring Link Attributes

SetTxPacketHeadroom

Reserves the specified number of bytes at the front of each packet.

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

SetWakeOnMagicPacketEnable

Enables or disables support for waking up the device when a specially formatted packet arrives.

IOUserNetworkMACAddress

A hardware address for a device.

