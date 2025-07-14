

- Core Motion
-  CMOdometerOriginDevice 

Enumeration

# CMOdometerOriginDevice

The device that the odometer sample originates from.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 10.15+visionOS 1.0+watchOS 8.4+

``` source
enum CMOdometerOriginDevice
```

## Topics

### Device origins

case unknown

The origin of the odometer sample is unknown.

case local

The origin of the odometer sample comes from the same device that requests the sample.

case remote

The origin of the odometer sample comes from a device that’s paired with the local device.

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

### Getting the device

var originDevice: CMOdometerOriginDevice

The device that measures the data.

