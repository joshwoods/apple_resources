

- Core Bluetooth
- CBCentralManagerState
-  CBCentralManagerState.resetting Deprecated

Case

# CBCentralManagerState.resetting

A state that indicates the connection with the system service was momentarily lost.

iOS 5.0–10.0DeprecatediPadOS 5.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.13DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–3.0Deprecated

``` source
case resetting
```

Deprecated

Use CBManagerState instead

## Discussion

This state indicates that Bluetooth is trying to reconnect. Once it does, Core Bluetooth updates the state value.

## See Also

### Constants

case poweredOff

A state that indicates Bluetooth is currently powered off.

Deprecated

case poweredOn

A state that indicates Bluetooth is currently powered on and available to use.

Deprecated

case unauthorized

A state that indicates the application isn’t authorized to use the Bluetooth low energy role.

Deprecated

case unknown

The manager’s state is unknown.

Deprecated

case unsupported

A state that indicates this device doesn’t support the Bluetooth low energy central or client role.

Deprecated

