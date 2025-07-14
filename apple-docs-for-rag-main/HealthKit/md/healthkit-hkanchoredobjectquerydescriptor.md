

- HealthKit
-  HKAnchoredObjectQueryDescriptor 

Structure

# HKAnchoredObjectQueryDescriptor

A query interface that runs anchored object queries using Swift concurrency.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct HKAnchoredObjectQueryDescriptor where Sample : HKSample
```

## Mentioned in 

Running Queries with Swift Concurrency

Reading data from HealthKit

## Overview

Use HKAnchoredObjectQueryDescriptor to read any changes to the HealthKit store that occurred after the provided anchor. When creating a new query descriptor, if you pass `nil` as the `anchor` parameter, the query reads all matching data from the store.

There are two common use cases for anchored object queries:

- Batch-read all the matching data from the HealthKit store using a series of HKAnchoredObjectQueryDescriptor instances.

- Monitor the HealthKit store for any changes to the matching data using a long-running HKAnchoredObjectQueryDescriptor instance.

### Batch Read Existing Data

Users may have large quantities of data saved to the HealthKit store; therefore, reading all data for a given data type might become very expensive, both in terms of memory usage and processing time. To avoid performance issues, you can use HKAnchoredObjectQueryDescriptor queries to read the data in batches.

Start with a `nil`-valued anchor, and create a one-shot query descriptor that reads a batch of data. After you process the results from one query, start a new one-shot query for the next batch. Continue reading batches until there’s no new data.

```
let stepType = HKQuantityType(.stepCount)

// Start by reading all matching data.
var anchor: HKQueryAnchor? = nil
var results: HKAnchoredObjectQueryDescriptor.Result

repeat {
    // Create a query descriptor that reads a batch
    // of 100 matching samples.
    let anchorDescriptor =
    HKAnchoredObjectQueryDescriptor(
        predicates: [.quantitySample(type: stepType)],
        anchor: anchor,
        limit: 100
    )

    results = try await anchorDescriptor.result(for: store)
    anchor = results.newAnchor

    // Process the batch of results here.

} while (results.addedSamples != []) && (results.deletedObjects != [])
```

Tip

Because HKQueryAnchor instances adopt the NSSecureCoding protocol, you can save the most recent anchor and use it the next time your app launches.

### Monitor for Changes

To monitor the HealthKit store for changes, start by creating an HKAnchoredObjectQueryDescriptor instance that matches the data you want to monitor. Pass in the anchor from the last time you read data from the HealthKit store.

Next, call the query descriptor’s results(for:) method to start your long-running query. This method returns an AsyncSequence instance which HealthKit uses to return `Results/Element` instances. The first result represents any changes currently in the HealthKit store, and additional results represent changes as they occur.

```
let stepType = HKQuantityType(.stepCount)

// Create a query descriptor.
let anchorDescriptor =
HKAnchoredObjectQueryDescriptor(
    predicates: [.quantitySample(type: stepType)],
    anchor: anchor
)

let updateQueue = anchorDescriptor.results(for: store)

updateTask = Task {
    for try await update in updateQueue {
        // Process the update here.
        print(update)
    }
}
```

## Topics

### Creating Query Descriptors

init(predicates: [HKSamplePredicate&lt;Sample>], anchor: HKQueryAnchor?, limit: Int?)

Creates an anchored object query descriptor.

### Running Queries

func result(for: HKHealthStore) async throws -> HKAnchoredObjectQueryDescriptor&lt;Sample>.Result

Runs a one-shot query and asynchronously returns a snapshot of the current matching results.

func results(for: HKHealthStore) -> HKAnchoredObjectQueryDescriptor&lt;Sample>.Results

Initiates a long-running query that returns its results using an asynchronous sequence.

struct Result

A set of results from an anchored object query.

struct Results

An asynchronous sequence that emits updates from an anchored object query.

### Accessing Query Properties

var predicates: [HKSamplePredicate&lt;Sample>]

A predicate that limits the results that the query returns.

var anchor: HKQueryAnchor?

An anchor that a previous anchored object query returned.

var limit: Int?

The maximum number of samples that the query returns.

### Default Implementations

HKAsyncQuery Implementations

HKAsyncSequenceQuery Implementations

## Relationships

### Conforms To

- Copyable
- HKAsyncQuery

  Conforms when `Sample` inherits `HKSample`.

- HKAsyncSequenceQuery

  Conforms when `Sample` inherits `HKSample`.

## See Also

### Long-running queries

struct HKActivitySummaryQueryDescriptor

A query interface that reads activity summaries using Swift concurrency.

class HKActivitySummaryQuery

A query for reading activity summary objects from the HealthKit store.

class HKAnchoredObjectQuery

A query that returns changes to the HealthKit store, including a snapshot of new changes and continuous monitoring as a long-running query.

class HKObserverQuery

A long-running query that monitors the HealthKit store and updates your app when the HealthKit store saves or deletes a matching sample.

