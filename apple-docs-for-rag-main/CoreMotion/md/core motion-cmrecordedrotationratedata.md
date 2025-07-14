

- Core Motion
-  CMRecordedRotationRateData 

Class

# CMRecordedRotationRateData

A data object that contains a single rotation-rate measurement at a specific time.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+watchOS 7.0+

``` source
class CMRecordedRotationRateData
```

## Topics

### Accessing Rotation Data

var startDate: Date

The time when the gyroscope measured the rotation data.

## Relationships

### Inherits From

- CMRotationRateData

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Getting the Rotation Rate

var rotationRate: CMRotationRate

The rotation rate as measured by the device’s gyroscope.

struct CMRotationRate

The type of structures representing a measurement of rotation rate.

class CMRotationRateData

A data object that contains a single rotation-rate measurement.

