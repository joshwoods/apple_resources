

- XCTest
- XCTPerformanceMeasurement
-  init(identifier:displayName:doubleValue:unitSymbol:) 

Initializer

# init(identifier:displayName:doubleValue:unitSymbol:)

Initializes a performance measurement for a single iteration with the value and unit of measurement.

``` source
init(
    identifier: String,
    displayName: String,
    doubleValue: Double,
    unitSymbol: String
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

## See Also

### Initializing a Measurement

convenience init(identifier: String, displayName: String, doubleValue: Double, unitSymbol: String, polarity: XCTPerformanceMeasurement.Polarity)

Initializes a performance measurement for a single iteration with the value, unit of measurement, and polarity.

convenience init(identifier: String, displayName: String, value: Measurement&lt;Unit>)

Initializes a performance measurement for a single iteration with the value.

convenience init(identifier: String, displayName: String, value: Measurement&lt;Unit>, polarity: XCTPerformanceMeasurement.Polarity)

Initializes a performance measurement for a single iteration with the value and polarity.

