

- HealthKit
- HKQuantitySample
-  count 

Instance Property

# count

The number of quantities contained in this sample.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 5.0+

``` source
var count: Int { get }
```

## Mentioned in 

Accessing condensed workout samples

## Discussion

Samples created using one of the `init()` methods have a count of `1`. Samples created using an HKQuantitySeriesSampleBuilder may have a count greater than `1`.

## See Also

### Related Documentation

class HKQuantitySeriesSampleQuery

A query that accesses the series data associated with a quantity sample.

### Getting Property Data

var quantity: HKQuantity

The quantity for this sample.

var quantityType: HKQuantityType

The quantity type for this sample.

