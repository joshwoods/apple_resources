

- MatterSupport
- MatterAddDeviceExtensionRequestHandler
- MatterAddDeviceExtensionRequestHandler.ThreadNetworkAssociation
-  network(extendedPANID:) 

Type Method

# network(extendedPANID:)

Obtains the Thread network extended PAN identifier.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
static func network(extendedPANID: UInt64) -> MatterAddDeviceExtensionRequestHandler.ThreadNetworkAssociation
```

## Return Value

The Thread network extended PAN identifier.

## Discussion

The system retrieves the network parameters from retrieveCredentials(forExtendedPANID:completion:) using the provided parameter. The credentials must be present in the store or else association and pairing fails.

## See Also

### Getting network information

static var defaultSystemNetwork: MatterAddDeviceExtensionRequestHandler.ThreadNetworkAssociation

A sentinel value to represent the system’s default Thread network.

