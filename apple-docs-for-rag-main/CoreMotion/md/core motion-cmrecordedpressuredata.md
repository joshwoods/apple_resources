

- Core Motion
-  CMRecordedPressureData 

Class

# CMRecordedPressureData

A recorded measurement of pressure data.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+watchOS 5.0+

``` source
class CMRecordedPressureData
```

## Overview

Use SensorKit’s ambientPressure sensor to read ambient pressure data.

## Topics

### Instance Properties

var identifier: UInt64

A value that uniquely identifies this measurement.

var startDate: Date

The time and date when the system recorded the measurement.

## Relationships

### Inherits From

- CMAmbientPressureData

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

### Ambient pressure

class CMAmbientPressureData

A measurement of the ambient pressure and temperature.

