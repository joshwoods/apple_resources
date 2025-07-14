

- XCTest
- XCTPerformanceMeasurement
-  identifier 

Instance Property

# identifier

A unique identifier for a measurement.

``` source
var identifier: String { get }
```

## Discussion

Make an identifier for a measurement unique to the property being measured; it doesn’t need to be unique for each instance of a measurement. As an example, a measurement of database access performance might have the identifier `com.example.ourdb_transactionthroughput`.

## See Also

### Identifying Measurements

var displayName: String

A human-readable name for a measurement.

