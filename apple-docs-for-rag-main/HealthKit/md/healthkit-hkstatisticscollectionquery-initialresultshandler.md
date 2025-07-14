

- HealthKit
- HKStatisticsCollectionQuery
-  initialResultsHandler 

Instance Property

# initialResultsHandler

The results handler for the query’s initial results.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
var initialResultsHandler: ((HKStatisticsCollectionQuery, HKStatisticsCollection?, (any Error)?) -> Void)? { get set }
```

## Discussion

If this property is not set to `nil`, the query executes the results handler on a background queue after it has finished calculating the statistics for all matching samples currently stored in HealthKit.

## See Also

### Getting and Setting Results Handlers

var statisticsUpdateHandler: ((HKStatisticsCollectionQuery, HKStatistics?, HKStatisticsCollection?, (any Error)?) -> Void)?

The results handler for monitoring updates to the HealthKit store.

