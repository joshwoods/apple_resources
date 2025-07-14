

- Core Bluetooth
- CBPeripheralManagerState
-  CBPeripheralManagerState.unknown Deprecated

Case

# CBPeripheralManagerState.unknown

A manager state that indicates the current state of the peripheral manager is unknown.

iOS 6.0–10.0DeprecatediPadOS 6.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.13DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–3.0Deprecated

``` source
case unknown
```

Deprecated

Use CBManagerState instead

## Discussion

When the manager is in this state, an update is imminent.

## See Also

### Constants

case resetting

A manager state that indicates the connection with the system service was momentarily lost.

Deprecated

case unsupported

A manager state that indicates the platform doesn’t support the Bluetooth low energy peripheral/server role.

Deprecated

case unauthorized

A manager state that indicates the app isn’t authorized to use the Bluetooth low energy peripheral/server role.

Deprecated

case poweredOff

A manager state that indicates Bluetooth is currently powered off.

Deprecated

case poweredOn

A manager state that indicates Bluetooth is currently powered on and is available to use.

Deprecated

