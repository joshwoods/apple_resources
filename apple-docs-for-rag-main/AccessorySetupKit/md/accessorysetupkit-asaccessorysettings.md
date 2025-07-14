

- AccessorySetupKit
-  ASAccessorySettings 

Class

# ASAccessorySettings

Properties of an accessory.

iOS 18.0+iPadOS 18.0+

``` source
class ASAccessorySettings
```

## Topics

### Applying default settings

class var `default`: ASAccessorySettings

An empty settings object.

### Inspecting accessory settings

var ssid: String?

A hotspot identifier that clients can use to connect to an accessory’s hotspot.

var bluetoothTransportBridgingIdentifier: Data?

A 6-byte identifier for bridging classic transport profiles.

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

### Managing authorization

func finishAuthorization(for: ASAccessory, settings: ASAccessorySettings, completionHandler: ((any Error)?) -> Void)

Finish authorization of a partially-setup accessory.

func failAuthorization(for: ASAccessory, completionHandler: ((any Error)?) -> Void)

End authorization of a partially-configured accessory as a failure.

