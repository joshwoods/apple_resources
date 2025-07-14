

- HealthKit
- HKStatisticsCollectionQueryDescriptor
-  options 

Instance Property

# options

A list of options that define the type of statistical calculations performed and the way in which HealthKit merges data from multiple sources.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
var options: HKStatisticsOptions
```

## See Also

### Accessing Query Properties

var predicate: HKSamplePredicate&lt;HKQuantitySample>

A predicate that defines the set of data that the query uses to calculate the statistics.

var anchorDate: Date

The date that anchors the collection’s time intervals.

var intervalComponents: DateComponents

The date components that define the time interval for each statistics object in the collection.

