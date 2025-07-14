

- NetworkingDriverKit
- IOUserNetworkEthernet
-  SetWakeOnMagicPacketEnable 

Instance Method

# SetWakeOnMagicPacketEnable

Enables or disables support for waking up the device when a specially formatted packet arrives.

DriverKit

``` source
kern_return_t SetWakeOnMagicPacketEnable(bool enable);
```

## Parameters 

`enable`  

If `YES`, enable promiscuous mode for the device; otherwise, disable it.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## Discussion

Override this method and use it to configure your driver’s wake-on-magic-packet support.

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

SetWakeOnMagicPacketSupport

Tells the system whether the device supports being woken up when a specially formatted packet arrives.

IOUserNetworkMACAddress

A hardware address for a device.

