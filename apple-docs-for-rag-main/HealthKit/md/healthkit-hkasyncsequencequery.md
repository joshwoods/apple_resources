

- HealthKit
-  HKAsyncSequenceQuery 

Protocol

# HKAsyncSequenceQuery

A protocol that defines a method for running queries that returns results using an asynchronous sequence.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
protocol HKAsyncSequenceQuery
```

## Mentioned in 

Running Queries with Swift Concurrency

## Topics

### Running Queries

associatedtype Sequence : AsyncSequence

The data type that the query returns.

**Required**

func results(for: HKHealthStore) -> Self.Sequence

Initiates a query that returns its results using an asynchronous sequence.

**Required**

## Relationships

### Conforming Types

- HKActivitySummaryQueryDescriptor
- HKAnchoredObjectQueryDescriptor

  Conforms when `Sample` inherits `HKSample`.

- HKElectrocardiogramQueryDescriptor
- HKHeartbeatSeriesQueryDescriptor
- HKQuantitySeriesSampleQueryDescriptor
- HKStatisticsCollectionQueryDescriptor
- HKWorkoutEffortRelationshipQueryDescriptor
- HKWorkoutRouteQueryDescriptor

## See Also

### Swift concurrency support

Running Queries with Swift Concurrency

Use Swift concurrency to manage one-shot and long-running queries.

protocol HKAsyncQuery

A protocol that defines an asynchronous method for running queries.

struct HKSamplePredicate

A predicate for queries that return a collection of matching sample objects.

