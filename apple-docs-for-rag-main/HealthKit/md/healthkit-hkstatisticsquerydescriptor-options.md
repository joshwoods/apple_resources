

- HealthKit
- HKStatisticsQueryDescriptor
-  options 

Instance Property

# options

A list of options that define the type of statistical calculations performed and the way in which HealthKit merges data from multiple sources.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
var options: HKStatisticsOptions
```

## Discussion

For a list of valid options, see HKStatisticsOptions.

## See Also

### Accessing Query Properties

var predicate: HKSamplePredicate&lt;HKQuantitySample>

A predicate that defines the set of data that the query uses to calculate the statistics.

