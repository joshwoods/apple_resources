

- HealthKit
- HKStatisticsCollectionQueryDescriptor
-  init(predicate:options:anchorDate:intervalComponents:) 

Initializer

# init(predicate:options:anchorDate:intervalComponents:)

Creates a statistics collection query descriptor.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
init(
    predicate: HKSamplePredicate,
    options: HKStatisticsOptions,
    anchorDate: Date,
    intervalComponents: DateComponents
)
```

## Parameters 

`predicate`  

A predicate that defines the set of data that the query uses to calculate the statistics.

`options`  

A list of options that define the type of statistical calculations performed and the way in which HealthKit merges data from multiple sources. For a list of valid options, see HKStatisticsOptions.

`anchorDate`  

The date anchors the collection’s time intervals. Use this parameter to set the start time for your time intervals. For example, if you’re using a day interval, you might create a date object with a time of 2:00 a.m. This value sets the start of the day for each of your time intervals.

Technically, the anchor sets the start time for a single time interval. All other time intervals must align with this interval. The time intervals can extend before or after the anchor date. Each time interval has the same length, and there’s no gap between adjacent intervals. Think of time as a number line: The anchor date represents its origin, and the intervals create tick marks that extend away from the origin in both directions.

`intervalComponents`  

The date components that define the time interval for each statistics object in the collection.

