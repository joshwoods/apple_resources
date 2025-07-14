

- HealthKit
-  HKAsyncQuery 

Protocol

# HKAsyncQuery

A protocol that defines an asynchronous method for running queries.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
protocol HKAsyncQuery
```

## Mentioned in 

Running Queries with Swift Concurrency

## Topics

### Running Queries

associatedtype Output

The type of data that the query returns.

**Required**

func result(for: HKHealthStore) async throws -> Self.Output

Runs a one-shot query and asynchronously returns a snapshot of the current matching results.

**Required**

## Relationships

### Conforming Types

- HKActivitySummaryQueryDescriptor
- HKAnchoredObjectQueryDescriptor

  Conforms when `Sample` inherits `HKSample`.

- HKSampleQueryDescriptor

  Conforms when `Sample` inherits `HKSample`.

- HKSourceQueryDescriptor

  Conforms when `Sample` inherits `HKSample`.

- HKStatisticsCollectionQueryDescriptor
- HKStatisticsQueryDescriptor
- HKVerifiableClinicalRecordQueryDescriptor
- HKWorkoutEffortRelationshipQueryDescriptor

## See Also

### Swift concurrency support

Running Queries with Swift Concurrency

Use Swift concurrency to manage one-shot and long-running queries.

protocol HKAsyncSequenceQuery

A protocol that defines a method for running queries that returns results using an asynchronous sequence.

struct HKSamplePredicate

A predicate for queries that return a collection of matching sample objects.

