

- Core Motion
-  CMRotationRateData 

Class

# CMRotationRateData

A data object that contains a single rotation-rate measurement.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+watchOS 7.0+

``` source
class CMRotationRateData
```

## Topics

### Accessing Rotation Data

var rotationRate: CMRotationRate

The rotation rate measured by the gyroscope.

## Relationships

### Inherits From

- CMLogItem

### Inherited By

- CMRecordedRotationRateData

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

class CMRecordedRotationRateData

A data object that contains a single rotation-rate measurement at a specific time.

