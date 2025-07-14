

- HealthKit
- HKQuantitySeriesSampleQuery
-  orderByQuantitySampleStartDate 

Instance Property

# orderByQuantitySampleStartDate

A Boolean value that determines whether the query groups the results based on the quantity sample’s start date.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var orderByQuantitySampleStartDate: Bool { get set }
```

## Discussion

By default the query returns all the quantities in ascending order based on their start date. If you set this property to true, HealthKit first sorts the matching HKQuantitySample objects by their startDate parameter. Then, for each sample, it returns all the quantity objects in ascending order. If the sample objects overlap, then the quantities may not appear in ascending order when switching from one sample to the next.

## See Also

### Creating a Series Query

init(quantityType: HKQuantityType, predicate: NSPredicate?, quantityHandler: (HKQuantitySeriesSampleQuery, HKQuantity?, DateInterval?, HKQuantitySample?, Bool, (any Error)?) -> Void)

Creates a new query for a series of the specified quantity type.

var includeSample: Bool

A Boolean value that determines whether the query should return the series sample.

