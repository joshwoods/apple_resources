

- HealthKit
- HKHealthStore
-  stop(\_:) 

Instance Method

# stop(\_:)

Stops a long-running query.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
func stop(_ query: HKQuery)
```

## Parameters 

`query`  

Either an HKObserverQuery instance or an HKStatisticsCollectionQuery instance.

## Mentioned in 

Reading route data

Executing Observer Queries

## Discussion

Use this method on long-running queries only. Most queries automatically stop after they have gathered the requested data. Long-running queries continue to operate on a background thread, watching the HealthKit store for updates. You can cancel these queries by using this method.

## See Also

### Querying HealthKit data

func execute(HKQuery)

Starts executing the provided query.

