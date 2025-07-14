

- XCTest
-  XCTPerformanceMeasurementTimestamp 

Class

# XCTPerformanceMeasurementTimestamp

A point in time that captures the start or finish of a performance test iteration.

``` source
class XCTPerformanceMeasurementTimestamp
```

## Topics

### Initializers

convenience init()

Intitializes a timestamp that represents the current time.

init(absoluteTime: UInt64, date: Date)

Intitializes a timestamp that represents the provided time.

### Mach Absolute Time

var absoluteTimeNanoSeconds: UInt64

The nanoseconds component of the absolute time.

var absoluteTime: UInt64

The absolute time of the timestamp, which is the value of the mach absolute time clock.

### Date

var date: Date

The timestamp’s representation as a date.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Measurements

class XCTPerformanceMeasurement

A measurement from a single iteration of a performance test.

