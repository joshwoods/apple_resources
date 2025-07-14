

- NetworkingDriverKit
- IOUserNetworkEthernet
-  SetAllMulticastModeEnable 

Instance Method

# SetAllMulticastModeEnable

Enables or disables multicast support for your service.

DriverKit

``` source
kern_return_t SetAllMulticastModeEnable(bool enable);
```

## Parameters 

`enable`  

If `YES`, enable multicast support on the device; otherwise, disable it.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## Discussion

Override this method and use it to enable multicast mode on your device.

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

SetPromiscuousModeEnable

Enables or disables support for monitoriong all network packets.

SetWakeOnMagicPacketSupport

Tells the system whether the device supports being woken up when a specially formatted packet arrives.

SetWakeOnMagicPacketEnable

Enables or disables support for waking up the device when a specially formatted packet arrives.

IOUserNetworkMACAddress

A hardware address for a device.

