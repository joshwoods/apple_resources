

- Core Bluetooth
- CBPeripheral
-  state 

Instance Property

# state

The connection state of the peripheral.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var state: CBPeripheralState { get }
```

## Discussion

This property represents the current connection state of the peripheral. For a list of the possible values, see CBPeripheralState.

## See Also

### Monitoring a Peripheral’s Connection State

enum CBPeripheralState

Values representing the connection state of a peripheral.

var canSendWriteWithoutResponse: Bool

A Boolean value that indicates whether the remote device can send a write without a response.

