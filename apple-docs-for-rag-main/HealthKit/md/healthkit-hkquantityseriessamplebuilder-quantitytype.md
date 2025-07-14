

- HealthKit
- HKQuantitySeriesSampleBuilder
-  quantityType 

Instance Property

# quantityType

The quantity type for the series.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 5.0+

``` source
@NSCopying
var quantityType: HKQuantityType { get }
```

## See Also

### Creating a Quantity Series Builder

init(healthStore: HKHealthStore, quantityType: HKQuantityType, startDate: Date, device: HKDevice?)

Creates a new quantity series builder.

var startDate: Date

The starting date and time for the sample.

var device: HKDevice?

The device providing the data.

