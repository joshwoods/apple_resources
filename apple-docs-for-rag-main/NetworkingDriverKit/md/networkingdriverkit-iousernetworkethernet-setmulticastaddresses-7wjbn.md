

- NetworkingDriverKit
- IOUserNetworkEthernet
-  SetMulticastAddresses 

Instance Method

# SetMulticastAddresses

Sets the device addresses to use for multicast filtering.

DriverKit

``` source
kern_return_t SetMulticastAddresses(const IOUserNetworkMACAddress * addresses, uint32_t count);
```

## Parameters 

`addresses`  

An array of MAC addresses for the devices to monitor.

`count`  

The number of items in the `addresses` parameter.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## Discussion

Override this method and use it to set up a Ethernet multicast filter on your device.

## See Also

### Configuring Link Attributes

SetTxPacketHeadroom

Reserves the specified number of bytes at the front of each packet.

SetTxPacketTailroom

Reserves the specified number of bytes at the end of each packet.

SetSoftwareVlanSupport

Enables software VLAN support.

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

