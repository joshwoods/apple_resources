

- XCTest
- XCTPerformanceMeasurement
-  init(identifier:displayName:value:polarity:) 

Initializer

# init(identifier:displayName:value:polarity:)

Initializes a performance measurement for a single iteration with the value and polarity.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
convenience init(
    identifier: String,
    displayName: String,
    value: Measurement,
    polarity: XCTPerformanceMeasurement.Polarity
)
```

## Parameters 

`identifier`  

A unique identifier for the measurement.

`displayName`  

A human-readable name for the measurement.

`value`  

A value for the measurement.

`polarity`  

A value that states whether larger or smaller measurements, relative to a set baseline, indicate better performance.

## See Also

### Initializing a Measurement

init(identifier: String, displayName: String, doubleValue: Double, unitSymbol: String)

Initializes a performance measurement for a single iteration with the value and unit of measurement.

convenience init(identifier: String, displayName: String, doubleValue: Double, unitSymbol: String, polarity: XCTPerformanceMeasurement.Polarity)

Initializes a performance measurement for a single iteration with the value, unit of measurement, and polarity.

convenience init(identifier: String, displayName: String, value: Measurement&lt;Unit>)

Initializes a performance measurement for a single iteration with the value.

