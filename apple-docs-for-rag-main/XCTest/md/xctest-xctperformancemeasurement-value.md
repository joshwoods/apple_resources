

- XCTest
- XCTPerformanceMeasurement
-  value 

Instance Property

# value

The measured value, including the unit of measure.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var value: Measurement { get }
```

## See Also

### Accessing Measured Values

var doubleValue: Double

The measured value.

var unitSymbol: String

A string that represents the unit of measurement.

var polarity: XCTPerformanceMeasurement.Polarity

A constant that states whether larger or smaller measurements, relative to a set baseline, indicate better performance.

enum Polarity

Constants that state whether larger or smaller measurements, relative to a set baseline, indicate better performance.

