

- Virtualization
- VZNetworkDevice
-  attachment 

Instance Property

# attachment

The network attachment that’s connected to this network device.

macOS 12.0+

``` source
var attachment: VZNetworkDeviceAttachment? { get set }
```

## Discussion

Setting this property results in an attempt to change the network device attachment which may fail. If the devices fails to attach, the system invokes virtualMachine(_:networkDevice:attachmentWasDisconnectedWithError:) and sets this property to `nil`. This property may change at any time while the VM is running based on the state of the host network.

