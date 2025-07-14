

- Core Bluetooth
-  CBPeripheralManagerState Deprecated

Enumeration

# CBPeripheralManagerState

Values that represent the current state of the peripheral manager.

iOS 6.0–10.0DeprecatediPadOS 6.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.13DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–3.0Deprecated

``` source
enum CBPeripheralManagerState
```

Deprecated

Use CBManagerState instead.

## Topics

### Constants

case unknown

A manager state that indicates the current state of the peripheral manager is unknown.

case resetting

A manager state that indicates the connection with the system service was momentarily lost.

case unsupported

A manager state that indicates the platform doesn’t support the Bluetooth low energy peripheral/server role.

case unauthorized

A manager state that indicates the app isn’t authorized to use the Bluetooth low energy peripheral/server role.

case poweredOff

A manager state that indicates Bluetooth is currently powered off.

case poweredOn

A manager state that indicates Bluetooth is currently powered on and is available to use.

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

### Deprecated

enum CBCentralManagerState

Values that represent the current state of a central manager object.

Deprecated

Deprecated Constants

This document describes the constants found in the Core Bluetooth framework.

