

- Core Bluetooth
- CBManagerState
-  CBManagerState.resetting 

Case

# CBManagerState.resetting

A state that indicates the connection with the system service was momentarily lost.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
case resetting
```

## Discussion

This state indicates that Bluetooth is trying to reconnect. After it reconnects, Core Bluetooth updates the state value.

## See Also

### Manager States

case poweredOff

A state that indicates Bluetooth is currently powered off.

case poweredOn

A state that indicates Bluetooth is currently powered on and available to use.

case unauthorized

A state that indicates the application isn’t authorized to use the Bluetooth low energy role.

case unknown

The manager’s state is unknown.

case unsupported

A state that indicates this device doesn’t support the Bluetooth low energy central or client role.

