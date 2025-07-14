

- HealthKit
- HKStatistics
-  quantityType 

Instance Property

# quantityType

The quantity type of the samples used to calculate these statistics.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var quantityType: HKQuantityType { get }
```

## Discussion

The quantity type from the statistics query used to generate these statistics.

## See Also

### Getting Property Data

var startDate: Date

The start of the time period included in these statistics.

var endDate: Date

The end of the time period included in these statistics.

var sources: [HKSource]?

An array containing all the sources contributing to these statistics.

