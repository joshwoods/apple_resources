

- Virtualization
- VZNetworkDeviceConfiguration
-  macAddress 

Instance Property

# macAddress

The media access control (MAC) address to assign to the network device.

macOS 11.0+

``` source
@NSCopying
var macAddress: VZMACAddress { get set }
```

## Discussion

The default value of this property is a random, locally administered, unicast address. Assign a custom value to this property if you want your network device to have a specific MAC address.

## See Also

### Setting configuration attributes

var attachment: VZNetworkDeviceAttachment?

The object that defines how the virtual network device communicates with the host system.

