

- MatterSupport
- MatterAddDeviceExtensionRequestHandler
- MatterAddDeviceExtensionRequestHandler.ThreadNetworkAssociation
-  defaultSystemNetwork 

Type Property

# defaultSystemNetwork

A sentinel value to represent the system’s default Thread network.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
static var defaultSystemNetwork: MatterAddDeviceExtensionRequestHandler.ThreadNetworkAssociation { get }
```

## See Also

### Getting network information

static func network(extendedPANID: UInt64) -> MatterAddDeviceExtensionRequestHandler.ThreadNetworkAssociation

Obtains the Thread network extended PAN identifier.

