

- NetworkingDriverKit
- IOUserNetworkEthernet
-  SetSoftwareVlanSupport 

Instance Method

# SetSoftwareVlanSupport

Enables software VLAN support.

DriverKit

``` source
kern_return_t SetSoftwareVlanSupport(bool isSupported);
```

## Parameters 

`isSupported`  

If `YES`, enable software VLAN support; otherwise, disable it.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## See Also

### Configuring Link Attributes

SetTxPacketHeadroom

Reserves the specified number of bytes at the front of each packet.

SetTxPacketTailroom

Reserves the specified number of bytes at the end of each packet.

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

