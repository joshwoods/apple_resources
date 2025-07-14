

- XCTest
-  XCTPerformanceMeasurement 

Class

# XCTPerformanceMeasurement

A measurement from a single iteration of a performance test.

``` source
class XCTPerformanceMeasurement
```

## Topics

### Initializing a Measurement

init(identifier: String, displayName: String, doubleValue: Double, unitSymbol: String)

Initializes a performance measurement for a single iteration with the value and unit of measurement.

convenience init(identifier: String, displayName: String, doubleValue: Double, unitSymbol: String, polarity: XCTPerformanceMeasurement.Polarity)

Initializes a performance measurement for a single iteration with the value, unit of measurement, and polarity.

convenience init(identifier: String, displayName: String, value: Measurement&lt;Unit>)

Initializes a performance measurement for a single iteration with the value.

convenience init(identifier: String, displayName: String, value: Measurement&lt;Unit>, polarity: XCTPerformanceMeasurement.Polarity)

Initializes a performance measurement for a single iteration with the value and polarity.

### Identifying Measurements

var displayName: String

A human-readable name for a measurement.

var identifier: String

A unique identifier for a measurement.

### Accessing Measured Values

var doubleValue: Double

The measured value.

var unitSymbol: String

A string that represents the unit of measurement.

var value: Measurement&lt;Unit>

The measured value, including the unit of measure.

var polarity: XCTPerformanceMeasurement.Polarity

A constant that states whether larger or smaller measurements, relative to a set baseline, indicate better performance.

enum Polarity

Constants that state whether larger or smaller measurements, relative to a set baseline, indicate better performance.

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

class XCTPerformanceMeasurementTimestamp

A point in time that captures the start or finish of a performance test iteration.

