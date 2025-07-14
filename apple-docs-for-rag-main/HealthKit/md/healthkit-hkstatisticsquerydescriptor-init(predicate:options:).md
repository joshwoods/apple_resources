

- HealthKit
- HKStatisticsQueryDescriptor
-  init(predicate:options:) 

Initializer

# init(predicate:options:)

Creates a statistics query descriptor.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
init(
    predicate: HKSamplePredicate,
    options: HKStatisticsOptions
)
```

## Parameters 

`predicate`  

A predicate that defines the set of data that the query uses to calculate the statistics.

`options`  

A list of options that define the type of statistical calculations performed and the way in which HealthKit merges data from multiple sources. For a list of valid options, see HKStatisticsOptions.

