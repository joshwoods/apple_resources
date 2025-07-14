

- HealthKit
-  HKActivitySummaryQueryDescriptor 

Structure

# HKActivitySummaryQueryDescriptor

A query interface that reads activity summaries using Swift concurrency.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct HKActivitySummaryQueryDescriptor
```

## Mentioned in 

Reading data from HealthKit

Running Queries with Swift Concurrency

## Overview

Use HKActivitySummaryQueryDescriptor to run a query that reads activity summary objects from the HealthKit store. To get a snapshot of activity summaries currently in the store, create a descriptor and call its result(for:) method.

```
// Get the start and end date components.
let calendar = Calendar(identifier: .gregorian)

var startComponents = calendar.dateComponents([.day, .month, .year], from: Date())
startComponents.hour = 0
startComponents.minute = 0
startComponents.second = 0

var endComponents = startComponents
endComponents.day = 1 + (endComponents.day ?? 0)

// Create a predicate for the query.
let today = HKQuery.predicate(forActivitySummariesBetweenStart: startComponents, end: endComponents)

// Create the descriptor.
let activeSummaryDescriptor = HKActivitySummaryQueryDescriptor(predicate:today)

// Run the query.
let results = try await activeSummaryDescriptor.result(for: store)
```

To set up a long-running query that returns both matching values currently in the HealthKit store, and any updates that arrive while the query is running, call the results(for:) method instead.

```
// Run a long-running query and monitor for updates.
let updateQueue = activeSummaryDescriptor.results(for: store)

// Wait for the initial results and updates.
updateTask = Task {
    for try await results in updateQueue {
        // Process results here.
    }
}
```

## Topics

### Creating query descriptors

init(predicate: NSPredicate?)

Instantiates an activity summary query descriptor.

### Running queries

func result(for: HKHealthStore) async throws -> [HKActivitySummary]

Runs a one-shot query and asynchronously returns a snapshot of the current matching results.

func results(for: HKHealthStore) -> HKActivitySummaryQueryDescriptor.Results

Initiates a long-running query that returns its results using an asynchronous sequence.

struct Results

An asynchronous sequence that emits updates from an activity summary query.

### Accessing query properties

var predicate: NSPredicate?

A predicate that limits the results that the query returned.

### Default Implementations

HKAsyncQuery Implementations

HKAsyncSequenceQuery Implementations

## Relationships

### Conforms To

- Copyable
- HKAsyncQuery
- HKAsyncSequenceQuery

## See Also

### Long-running queries

class HKActivitySummaryQuery

A query for reading activity summary objects from the HealthKit store.

struct HKAnchoredObjectQueryDescriptor

A query interface that runs anchored object queries using Swift concurrency.

class HKAnchoredObjectQuery

A query that returns changes to the HealthKit store, including a snapshot of new changes and continuous monitoring as a long-running query.

class HKObserverQuery

A long-running query that monitors the HealthKit store and updates your app when the HealthKit store saves or deletes a matching sample.

