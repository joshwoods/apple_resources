

- Core Bluetooth
-  CBCentralManagerState Deprecated

Enumeration

# CBCentralManagerState

Values that represent the current state of a central manager object.

iOS 5.0–10.0DeprecatediPadOS 5.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.13DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–3.0Deprecated

``` source
enum CBCentralManagerState
```

Deprecated

Use CBManagerState instead.

## Topics

### Constants

case poweredOff

A state that indicates Bluetooth is currently powered off.

case poweredOn

A state that indicates Bluetooth is currently powered on and available to use.

case resetting

A state that indicates the connection with the system service was momentarily lost.

case unauthorized

A state that indicates the application isn’t authorized to use the Bluetooth low energy role.

case unknown

The manager’s state is unknown.

case unsupported

A state that indicates this device doesn’t support the Bluetooth low energy central or client role.

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

enum CBPeripheralManagerState

Values that represent the current state of the peripheral manager.

Deprecated

Deprecated Constants

This document describes the constants found in the Core Bluetooth framework.

