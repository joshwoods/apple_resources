

- HealthKit
-  HKStatisticsQueryDescriptor 

Structure

# HKStatisticsQueryDescriptor

A query descriptor that calculates the minimum, maximum, average, or sum over a set of samples from the HealthKit store.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct HKStatisticsQueryDescriptor
```

## Mentioned in 

Reading data from HealthKit

## Overview

Use the HKStatisticsQueryDescriptor to perform calculations over sets of samples currently saved in the HealthKit store.

```
// Create a predicate for today's samples.
let calendar = Calendar(identifier: .gregorian)
let startDate = calendar.startOfDay(for: Date())
let endDate = calendar.date(byAdding: .day, value: 1, to: startDate)
let today = HKQuery.predicateForSamples(withStart: startDate, end: endDate)

// Create the query descriptor.
let stepType = HKQuantityType(.stepCount)
let stepsToday = HKSamplePredicate.quantitySample(type: stepType, predicate:today)
let sumOfStepsQuery = HKStatisticsQueryDescriptor(predicate: stepsToday, options: .cumulativeSum)

// Run the query.
let stepCount = try await sumOfStepsQuery.result(for: store)?
    .sumQuantity()?
    .doubleValue(for: HKUnit.count())

// Use the step count here.
```

## Topics

### Creating Query Descriptors

init(predicate: HKSamplePredicate&lt;HKQuantitySample>, options: HKStatisticsOptions)

Creates a statistics query descriptor.

### Running Queries

func result(for: HKHealthStore) async throws -> HKStatistics?

Runs a one-shot query and asynchronously returns a snapshot of the current matching results.

### Accessing Query Properties

var predicate: HKSamplePredicate&lt;HKQuantitySample>

A predicate that defines the set of data that the query uses to calculate the statistics.

var options: HKStatisticsOptions

A list of options that define the type of statistical calculations performed and the way in which HealthKit merges data from multiple sources.

### Default Implementations

HKAsyncQuery Implementations

## Relationships

### Conforms To

- Copyable
- HKAsyncQuery

## See Also

### Statistics

Executing Statistical Queries

Create and run statistical queries.

Executing Statistics Collection Queries

Calculate statistical data for graphs and charts.

class HKStatisticsQuery

A query that performs statistical calculations over a set of matching quantity samples, and returns the results.

struct HKStatisticsCollectionQueryDescriptor

A query descriptor that gathers a collection of statistics calculated over a series of fixed-length time intervals.

class HKStatisticsCollectionQuery

A query that performs multiple statistics queries over a series of fixed-length time intervals.

class HKStatistics

An object that represents the result of calculating the minimum, maximum, average, or sum over a set of samples from the HealthKit store.

class HKStatisticsCollection

An object that manages a collection of statistics, representing the results calculated over separate time intervals.

struct HKStatisticsOptions

Options for specifying the statistic to calculate.

