

- Core Motion
- CMDeviceMotion
-  CMDeviceMotion.SensorLocation 

Enumeration

# CMDeviceMotion.SensorLocation

Defines the device’s sensor locations.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
enum SensorLocation
```

## Topics

### Sensor Locations

case `default`

The default sensor location.

case headphoneLeft

The sensor is in the left headphone.

case headphoneRight

The sensor is in the right headphone.

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

### Getting the Sensor Location

var sensorLocation: CMDeviceMotion.SensorLocation

The location of the sensors that compute the device-motion data.

