

- HealthKit
- HKQuantitySeriesSampleBuilder
-  device 

Instance Property

# device

The device providing the data.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 5.0+

``` source
@NSCopying
var device: HKDevice? { get }
```

## See Also

### Creating a Quantity Series Builder

init(healthStore: HKHealthStore, quantityType: HKQuantityType, startDate: Date, device: HKDevice?)

Creates a new quantity series builder.

var quantityType: HKQuantityType

The quantity type for the series.

var startDate: Date

The starting date and time for the sample.

