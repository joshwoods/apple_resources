

- HealthKit
- HKStatisticsCollectionQuery
-  statisticsUpdateHandler 

Instance Property

# statisticsUpdateHandler

The results handler for monitoring updates to the HealthKit store.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
var statisticsUpdateHandler: ((HKStatisticsCollectionQuery, HKStatistics?, HKStatisticsCollection?, (any Error)?) -> Void)? { get set }
```

## Discussion

If this property is set to `nil`, the statistics collection query will automatically stop as soon as it has finished calculating the initial results. If this property is not `nil`, the query behaves similarly to the observer query. It continues to run, monitoring the HealthKit store. If any new, matching samples are saved to the store—or if any of the existing matching samples are deleted from the store—the query executes the update handler on a background queue.

## See Also

### Getting and Setting Results Handlers

var initialResultsHandler: ((HKStatisticsCollectionQuery, HKStatisticsCollection?, (any Error)?) -> Void)?

The results handler for the query’s initial results.

