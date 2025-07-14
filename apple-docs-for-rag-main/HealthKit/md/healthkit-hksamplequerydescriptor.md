

- HealthKit
-  HKSampleQueryDescriptor 

Structure

# HKSampleQueryDescriptor

A query interface that reads samples using Swift concurrency.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct HKSampleQueryDescriptor where Sample : HKSample
```

## Mentioned in 

Reading data from HealthKit

Running Queries with Swift Concurrency

## Overview

Use HKSampleQueryDescriptor to run a general query that returns a snapshot of all the matching samples currently saved in the HealthKit store.

```
// Define the type.
let stepType = HKQuantityType(.stepCount)

// Create the descriptor.
let descriptor = HKSampleQueryDescriptor(
    predicates:[.quantitySample(type: stepType)],
    sortDescriptors: [SortDescriptor(\.endDate, order: .reverse)],
    limit: 10)

// Launch the query and wait for the results.
// The system automatically sets results to [HKQuantitySample].
let results = try await descriptor.result(for: store)

for result in results {
    // Process the results here.
}
```

When you call the descriptor’s result(for:) method, it creates and executes an HKSampleQuery in the background, passing the results from the query’s `resultsHandler` as its return value.

## Topics

### Creating Query Descriptors

init(predicates: [HKSamplePredicate&lt;Sample>], sortDescriptors: [SortDescriptor&lt;Sample>], limit: Int?)

Creates a sample query descriptor.

### Running Queries

func result(for: HKHealthStore) async throws -> [Sample]

Runs a one-shot query and asynchronously returns a snapshot of the current matching results.

### Accessing Query Properties

var limit: Int?

The maximum number of samples that the query returns.

var predicates: [HKSamplePredicate&lt;Sample>]

An array of sample predicates that define the type of data that the query returns.

var sortDescriptors: [SortDescriptor&lt;Sample>]

An array that specifies the order of the results that the query returns.

### Default Implementations

HKAsyncQuery Implementations

## Relationships

### Conforms To

- Copyable
- HKAsyncQuery

  Conforms when `Sample` inherits `HKSample`.

## See Also

### Basic queries

class HKSampleQuery

A general query that returns a snapshot of all the matching samples currently saved in the HealthKit store.

class HKCorrelationQuery

A query that performs complex searches based on the correlation’s contents, and returns a snapshot of all matching samples.

class HKQueryDescriptor

A descriptor that specifies a set of samples based on the data type and a predicate.

class HKQuery

An abstract class for all the query classes in HealthKit.

