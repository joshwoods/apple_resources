

- Core Bluetooth
-  CBPeripheralState 

Enumeration

# CBPeripheralState

Values representing the connection state of a peripheral.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum CBPeripheralState
```

## Topics

### Peripheral States

case disconnected

The peripheral isn’t connected to the central manager.

case connecting

The peripheral is in the process of connecting to the central manager.

case connected

The peripheral is connected to the central manager.

case disconnecting

The peripheral is disconnecting from the central manager.

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

### Monitoring a Peripheral’s Connection State

var state: CBPeripheralState

The connection state of the peripheral.

var canSendWriteWithoutResponse: Bool

A Boolean value that indicates whether the remote device can send a write without a response.

