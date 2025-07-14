

- Core Bluetooth
-  CBPeripheralManagerConnectionLatency 

Enumeration

# CBPeripheralManagerConnectionLatency

Values representing the connection latency of the peripheral manager.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum CBPeripheralManagerConnectionLatency
```

## Topics

### Latency Values

case low

A latency setting indicating that prioritizes rapid communication over battery life.

case medium

A latency setting that balances communication frequency and battery life.

case high

A latency setting that prioritizes extending battery life over rapid communication.

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

### Setting Connection Latency

func setDesiredConnectionLatency(CBPeripheralManagerConnectionLatency, for: CBCentral)

Sets the desired connection latency for an existing connection to a central device.

