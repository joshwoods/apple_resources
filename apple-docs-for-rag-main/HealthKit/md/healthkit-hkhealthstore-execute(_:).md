

- HealthKit
- HKHealthStore
-  execute(\_:) 

Instance Method

# execute(\_:)

Starts executing the provided query.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
func execute(_ query: HKQuery)
```

## Parameters 

`query`  

A concrete subclass of the HKQuery class (any of the classes HKSampleQuery, HKAnchoredObjectQuery, HKCorrelationQuery, HKObserverQuery, HKSourceQuery, HKStatisticsQuery, or HKStatisticsCollectionQuery).

## Mentioned in 

Executing Anchored Object Queries

Executing Observer Queries

Executing Sample Queries

Executing Statistical Queries

Executing Source Queries

## Discussion

HealthKit executes queries asynchronously on a background queue. Most queries automatically stop after they have finished executing. However, long-running queries—such as observer queries and some statistics collection queries—continue to execute in the background. To stop long-running queries, call the stop(_:) method.

## See Also

### Querying HealthKit data

func stop(HKQuery)

Stops a long-running query.

