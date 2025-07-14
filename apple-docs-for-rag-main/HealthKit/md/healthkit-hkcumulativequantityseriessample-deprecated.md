

- HealthKit
-  HKCumulativeQuantitySeriesSample Deprecated

Class

# HKCumulativeQuantitySeriesSample

A sample representing a series of cumulative quantity values.

iOS 12.0–13.0DeprecatediPadOS 12.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOSvisionOS 1.0–1.0DeprecatedwatchOS 5.0–6.0Deprecated

``` source
class HKCumulativeQuantitySeriesSample
```

Deprecated

Use HKCumulativeQuantitySample instead.

## Topics

### Accessing Data

var sum: HKQuantity

The sum of all the quantities in the series.

### Specifying Predicate Key Paths

let HKPredicateKeyPathSum: String

The key path for accessing the sum of a quantity series inside a predicate format string.

## Relationships

### Inherits From

- HKCumulativeQuantitySample

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Related Documentation

class HKQuantitySeriesSampleQuery

A query that accesses the series data associated with a quantity sample.

