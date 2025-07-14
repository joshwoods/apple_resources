

- Core Bluetooth
-  CBPeripheralManagerAuthorizationStatus Deprecated

Enumeration

# CBPeripheralManagerAuthorizationStatus

Values representing the current authorization state of the peripheral manager.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–6.0Deprecated

``` source
enum CBPeripheralManagerAuthorizationStatus
```

Deprecated

Use CBManagerAuthorization instead

## Topics

### Constants

case notDetermined

An authorization status that indicates the user hasn’t indicated whether this app can share data using Bluetooth while in the background.

case restricted

An authorization status that indicates this app isn’t authorized to share data using Bluetooth while in the background.

case denied

An authorization status that indicates the user explicitly denied this app from sharing data using Bluetooth while in the background.

case authorized

An authorization status that indicates the user authorized this app to share data using Bluetooth while in the background.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Monitoring the State of a Peripheral Manager

class func authorizationStatus() -> CBPeripheralManagerAuthorizationStatus

Returns the app’s authorization status for sharing data while in the background.

Deprecated

enum CBPeripheralManagerState

Values that represent the current state of the peripheral manager.

Deprecated

