

- HealthKit
- HKStatisticsCollectionQuery
-  init(quantityType:quantitySamplePredicate:options:anchorDate:intervalComponents:) 

Initializer

# init(quantityType:quantitySamplePredicate:options:anchorDate:intervalComponents:)

Initializes a statistics collection query to perform the specified calculations over a set of time intervals.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
init(
    quantityType: HKQuantityType,
    quantitySamplePredicate: NSPredicate?,
    options: HKStatisticsOptions = [],
    anchorDate: Date,
    intervalComponents: DateComponents
)
```

## Parameters 

`quantityType`  

The type of sample to search for. This type must be an instance of the HKQuantityType class. You cannot perform statistics collection queries using other sample types.

`quantitySamplePredicate`  

A predicate that limits the results returned by the query. You can pass `nil` if you want to perform the statistical calculation over all the samples of the specified type.

`options`  

A list of options that define the type of statistical calculations performed and the way in which data from multiple sources are merged. For a list of valid options, see HKStatisticsOptions.

`anchorDate`  

The date used to anchor the collection’s time intervals. Use this parameter to set the start time for your time intervals. For example, if you are using a day interval, you might create a date object with a time of 2:00 a.m. This value sets the start of the day for each of your time intervals.

Technically, the anchor sets the start time for a single time interval. All other time intervals must align with this interval. The time intervals can extend before or after the anchor date. Each time interval has the same length, and there is no gap between adjacent intervals. Think of time as a number line: The anchor date represents its origin, with the intervals creating tick marks that extend away from the origin in both directions.

`intervalComponents`  

The date components that define the time interval for each statistics object in the collection. For a collection of sample time intervals, see intervalComponents.

## Return Value

A newly initialized statistics collection query object.

## Discussion

After you instantiate the query, set up one or both of the callback handlers, and then call the HKHealthStore class’s execute(_:) method to run it. Queries run on an anonymous background queue. As soon as the query is complete, the initial results handler is executed on the same background queue (but not necessarily on the same thread). You typically dispatch these results to the main queue to update the user interface.

Statistics collection queries can also act as long-running queries. If you assign a statistics update handler, they continue to monitor the HealthKit store after gathering the initial results. The statistics update handler is called on the background queue every time a matching sample is saved to the HealthKit Store. You can cancel this query by calling the store’s stop(_:) method.

Note

Statistical calculations can take a considerable amount of time, especially if there are a large number of samples involved.

## See Also

### Related Documentation

var statisticsUpdateHandler: ((HKStatisticsCollectionQuery, HKStatistics?, HKStatisticsCollection?, (any Error)?) -> Void)?

The results handler for monitoring updates to the HealthKit store.

var anchorDate: Date

The anchor date for the collection’s time intervals.

var intervalComponents: DateComponents

The date components that define the time interval for each statistics object in the collection.

var options: HKStatisticsOptions

A list of options that define the type of statistical calculations performed and the way in which data from multiple sources are merged.

var initialResultsHandler: ((HKStatisticsCollectionQuery, HKStatisticsCollection?, (any Error)?) -> Void)?

The results handler for the query’s initial results.

### Creating Statistics Collection Objects

Executing Statistics Collection Queries

Calculate statistical data for graphs and charts.

