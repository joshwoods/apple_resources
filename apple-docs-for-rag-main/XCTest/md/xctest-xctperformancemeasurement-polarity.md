

- XCTest
- XCTPerformanceMeasurement
-  polarity 

Instance Property

# polarity

A constant that states whether larger or smaller measurements, relative to a set baseline, indicate better performance.

``` source
var polarity: XCTPerformanceMeasurement.Polarity { get }
```

## See Also

### Accessing Measured Values

var doubleValue: Double

The measured value.

var unitSymbol: String

A string that represents the unit of measurement.

var value: Measurement&lt;Unit>

The measured value, including the unit of measure.

enum Polarity

Constants that state whether larger or smaller measurements, relative to a set baseline, indicate better performance.

