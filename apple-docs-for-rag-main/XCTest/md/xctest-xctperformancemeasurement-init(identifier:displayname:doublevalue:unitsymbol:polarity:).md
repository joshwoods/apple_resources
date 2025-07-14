

- XCTest
- XCTPerformanceMeasurement
-  init(identifier:displayName:doubleValue:unitSymbol:polarity:) 

Initializer

# init(identifier:displayName:doubleValue:unitSymbol:polarity:)

Initializes a performance measurement for a single iteration with the value, unit of measurement, and polarity.

``` source
convenience init(
    identifier: String,
    displayName: String,
    doubleValue: Double,
    unitSymbol: String,
    polarity: XCTPerformanceMeasurement.Polarity
)
```

## Parameters 

`identifier`  

A unique identifier for the measurement.

`displayName`  

A human-readable name for the measurement.

`doubleValue`  

A value for the measurement.

`unitSymbol`  

A string that represents the unit of measurement, such as seconds.

`polarity`  

A value that states whether larger or smaller measurements, relative to a set baseline, indicate better performance.

## See Also

### Initializing a Measurement

init(identifier: String, displayName: String, doubleValue: Double, unitSymbol: String)

Initializes a performance measurement for a single iteration with the value and unit of measurement.

convenience init(identifier: String, displayName: String, value: Measurement&lt;Unit>)

Initializes a performance measurement for a single iteration with the value.

convenience init(identifier: String, displayName: String, value: Measurement&lt;Unit>, polarity: XCTPerformanceMeasurement.Polarity)

Initializes a performance measurement for a single iteration with the value and polarity.

