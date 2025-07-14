

- XCTest
- XCTPerformanceMeasurement
-  unitSymbol 

Instance Property

# unitSymbol

A string that represents the unit of measurement.

``` source
var unitSymbol: String { get }
```

## See Also

### Accessing Measured Values

var doubleValue: Double

The measured value.

var value: Measurement&lt;Unit>

The measured value, including the unit of measure.

var polarity: XCTPerformanceMeasurement.Polarity

A constant that states whether larger or smaller measurements, relative to a set baseline, indicate better performance.

enum Polarity

Constants that state whether larger or smaller measurements, relative to a set baseline, indicate better performance.

