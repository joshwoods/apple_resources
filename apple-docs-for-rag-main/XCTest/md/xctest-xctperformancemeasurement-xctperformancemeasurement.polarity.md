

- XCTest
- XCTPerformanceMeasurement
-  XCTPerformanceMeasurement.Polarity 

Enumeration

# XCTPerformanceMeasurement.Polarity

Constants that state whether larger or smaller measurements, relative to a set baseline, indicate better performance.

``` source
enum Polarity
```

## Topics

### Polarity Types

case prefersLarger

A performance measurement where a larger value, relative to a set baseline, indicates better performance.

case prefersSmaller

A performance measurement where a smaller value, relative to a set baseline, indicates better performance.

case unspecified

A performance measurement that doesn’t specify whether a larger or smaller value, relative to a set baseline, indicates better performance.

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

### Accessing Measured Values

var doubleValue: Double

The measured value.

var unitSymbol: String

A string that represents the unit of measurement.

var value: Measurement&lt;Unit>

The measured value, including the unit of measure.

var polarity: XCTPerformanceMeasurement.Polarity

A constant that states whether larger or smaller measurements, relative to a set baseline, indicate better performance.

