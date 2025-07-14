

- AccessorySetupKit
-  ASAccessory 

Class

# ASAccessory

An accessory discovered by the accessory session.

iOS 18.0+iPadOS 18.0+

``` source
class ASAccessory
```

## Topics

### Accessing identifiers

var bluetoothIdentifier: UUID?

The accessory’s unique Bluetooth identifier, if any.

var bluetoothTransportBridgingIdentifier: Data?

The accessory’s Bluetooth identifier, if any, for use when bridging classic transport profiles.

var ssid: String?

The accessory’s Wi-Fi SSID, if any.

### Presenting a display name

var displayName: String

The accessory’s name, suitable for displaying to someone using your app.

### Inspecting the accessory’s descriptor

var descriptor: ASDiscoveryDescriptor

The descriptor used to discover the accessory.

### Inspecting accessory state

var state: ASAccessory.AccessoryState

The current authorization state of the accessory.

enum AccessoryState

An enumeration of possible authorization states of an accessory.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Accessory description

enum AccessoryState

An enumeration of possible authorization states of an accessory.

