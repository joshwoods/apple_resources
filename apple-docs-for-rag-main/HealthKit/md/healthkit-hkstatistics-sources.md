

- HealthKit
- HKStatistics
-  sources 

Instance Property

# sources

An array containing all the sources contributing to these statistics.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
var sources: [HKSource]? { get }
```

## Discussion

If the separateBySource option was specified, this property holds an array of all the sources included in the calculations. If the separateBySource option was not specified, the property contains `nil`.

## See Also

### Getting Property Data

var startDate: Date

The start of the time period included in these statistics.

var endDate: Date

The end of the time period included in these statistics.

var quantityType: HKQuantityType

The quantity type of the samples used to calculate these statistics.

