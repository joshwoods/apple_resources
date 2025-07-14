

- HealthKit
-  HKStatisticsCollectionQueryDescriptor 

Structure

# HKStatisticsCollectionQueryDescriptor

A query descriptor that gathers a collection of statistics calculated over a series of fixed-length time intervals.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct HKStatisticsCollectionQueryDescriptor
```

## Mentioned in 

Reading data from HealthKit

Running Queries with Swift Concurrency

## Overview

Use HKStatisticsCollectionQueryDescriptor to run a query that calculates statistics grouped into time intervals. To get a snapshot of the current data in the store, create a descriptor and call its result(for:) method.

```
// Create a predicate for this week's samples.
let calendar = Calendar(identifier: .gregorian)
let today = calendar.startOfDay(for: Date())

guard let endDate = calendar.date(byAdding: .day, value: 1, to: today) else {
    fatalError("*** Unable to calculate the end time ***")
}

guard let startDate = calendar.date(byAdding: .day, value: -7, to: endDate) else {
    fatalError("*** Unable to calculate the start time ***")
}

let thisWeek = HKQuery.predicateForSamples(withStart: startDate, end: endDate)

// Create the query descriptor.
let stepType = HKQuantityType(.stepCount)
let stepsThisWeek = HKSamplePredicate.quantitySample(type: stepType, predicate:thisWeek)
let everyDay = DateComponents(day:1)

let sumOfStepsQuery = HKStatisticsCollectionQueryDescriptor(
    predicate: stepsThisWeek,
    options: .cumulativeSum,
    anchorDate: endDate,
    intervalComponents: everyDay)

let stepCounts = try await sumOfStepsQuery.result(for: store)

// Use the statistics collection here.
```

To set up a long-running query that updates the calculations based on any new data that arrives while it’s running, call the results(for:) method instead. The first result contains calculations based on samples currently in the HealthKit store, and additional results represent updates as they occur.

```
// Run a long-running query that updates its statistics as new data comes in.
let updateQueue = sumOfStepsQuery.results(for: store)

// Wait for the initial results and updates.
updateTask = Task {
    for try await results in updateQueue {
        // Use the statistics collection here.
    }
}
```

## Topics

### Creating Query Descriptors

init(predicate: HKSamplePredicate&lt;HKQuantitySample>, options: HKStatisticsOptions, anchorDate: Date, intervalComponents: DateComponents)

Creates a statistics collection query descriptor.

### Running Queries

func result(for: HKHealthStore) async throws -> HKStatisticsCollection

Runs a one-shot query and asynchronously returns statistics calculated from the current matching results.

func results(for: HKHealthStore) -> HKStatisticsCollectionQueryDescriptor.Results

Initiates a long-running query that returns statistics and updates using an asynchronous sequence.

struct Results

An asynchronous sequence that emits updates from a statistics collection query.

### Accessing Query Properties

var predicate: HKSamplePredicate&lt;HKQuantitySample>

A predicate that defines the set of data that the query uses to calculate the statistics.

var options: HKStatisticsOptions

A list of options that define the type of statistical calculations performed and the way in which HealthKit merges data from multiple sources.

var anchorDate: Date

The date that anchors the collection’s time intervals.

var intervalComponents: DateComponents

The date components that define the time interval for each statistics object in the collection.

### Structures

struct Result

A collection of results.

### Default Implementations

HKAsyncQuery Implementations

HKAsyncSequenceQuery Implementations

## Relationships

### Conforms To

- Copyable
- HKAsyncQuery
- HKAsyncSequenceQuery

## See Also

### Statistics

Executing Statistical Queries

Create and run statistical queries.

Executing Statistics Collection Queries

Calculate statistical data for graphs and charts.

struct HKStatisticsQueryDescriptor

A query descriptor that calculates the minimum, maximum, average, or sum over a set of samples from the HealthKit store.

class HKStatisticsQuery

A query that performs statistical calculations over a set of matching quantity samples, and returns the results.

class HKStatisticsCollectionQuery

A query that performs multiple statistics queries over a series of fixed-length time intervals.

class HKStatistics

An object that represents the result of calculating the minimum, maximum, average, or sum over a set of samples from the HealthKit store.

class HKStatisticsCollection

An object that manages a collection of statistics, representing the results calculated over separate time intervals.

struct HKStatisticsOptions

Options for specifying the statistic to calculate.

