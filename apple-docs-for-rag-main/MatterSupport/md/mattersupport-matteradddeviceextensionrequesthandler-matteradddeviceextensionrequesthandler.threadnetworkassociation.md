

- MatterSupport
- MatterAddDeviceExtensionRequestHandler
-  MatterAddDeviceExtensionRequestHandler.ThreadNetworkAssociation 

Structure

# MatterAddDeviceExtensionRequestHandler.ThreadNetworkAssociation

The description of an association to a Thread network.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
struct ThreadNetworkAssociation
```

## Topics

### Getting network information

static var defaultSystemNetwork: MatterAddDeviceExtensionRequestHandler.ThreadNetworkAssociation

A sentinel value to represent the system’s default Thread network.

static func network(extendedPANID: UInt64) -> MatterAddDeviceExtensionRequestHandler.ThreadNetworkAssociation

Obtains the Thread network extended PAN identifier.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Selecting the Thread network

func selectThreadNetwork(from: [MatterAddDeviceExtensionRequestHandler.ThreadScanResult]) async throws -> MatterAddDeviceExtensionRequestHandler.ThreadNetworkAssociation

Provides the visible Thread networks to the device.

struct ThreadScanResult

A result of a Thread-scan operation performed on the device

