

- Virtualization
- VZNetworkDeviceConfiguration
-  attachment 

Instance Property

# attachment

The object that defines how the virtual network device communicates with the host system.

macOS 11.0+

``` source
var attachment: VZNetworkDeviceAttachment? { get set }
```

## Discussion

The default value of this property is `nil`. Assign an appropriate value to specify the type of network interface you want to make available to the guest operating system. For example, assign a VZBridgedNetworkDeviceAttachment object to grant access to one of the host computer’s physical network interfaces.

Important

If you assign a VZBridgedNetworkDeviceAttachment object to this property, your app must have the com.apple.vm.networking entitlement. Without that entitlement, validation of your VZVirtualMachineConfiguration object fails.

## See Also

### Setting configuration attributes

var macAddress: VZMACAddress

The media access control (MAC) address to assign to the network device.

