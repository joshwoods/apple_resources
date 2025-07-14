

- Core Bluetooth
- CBPeripheral
-  canSendWriteWithoutResponse 

Instance Property

# canSendWriteWithoutResponse

A Boolean value that indicates whether the remote device can send a write without a response.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var canSendWriteWithoutResponse: Bool { get }
```

## Discussion

If this value is false, flushing all current writes sets the value to true. This also results in a call to the delegate’s peripheralIsReady(toSendWriteWithoutResponse:).

## See Also

### Monitoring a Peripheral’s Connection State

var state: CBPeripheralState

The connection state of the peripheral.

enum CBPeripheralState

Values representing the connection state of a peripheral.

