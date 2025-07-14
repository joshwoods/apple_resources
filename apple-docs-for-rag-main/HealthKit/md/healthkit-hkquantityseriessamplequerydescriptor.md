

- HealthKit
-  HKQuantitySeriesSampleQueryDescriptor 

Structure

# HKQuantitySeriesSampleQueryDescriptor

A query interface that reads the series data associated with quantity samples using Swift concurrency.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct HKQuantitySeriesSampleQueryDescriptor
```

## Overview

Use HKQuantitySeriesSampleQueryDescriptor to read the series data included in quantity samples. Apps can save any quantity data as a series using the HKQuantitySeriesSampleBuilder class; however, series data typically comes from high-frequency data saved during a workout. Any HKQuantitySample that has a count greater than `1` contains series data.

Important

Only use this query when you need direct access to the high-frequency series data, for example when visualizing the raw data or when exporting objects from the HealthKit store. For most common calculations, consider using a statistical query instead. Statistical queries correctly handle quantity data, whether the samples represent a single quantity or a series.

To read the individual data entries, create a predicate that identifies the sample type and limits the results to the desired data. For example, to read the series for a particular sample object, include a predicateForObject(with:) predicate. However, if you’re reading high-frequency data during a workout, you may want to include a predicateForSamples(withStart:end:options:) predicate that returns matching series data based on the workout’s time period instead.

```
// Create the predicate for the data.
let heartRate = HKQuantityType(.heartRate)
let objectPredicate = HKQuery.predicateForObject(with: myHeartRateSample.uuid)
let predicate = HKSamplePredicate.quantitySample(type: heartRate,
                                                 predicate: objectPredicate)

// Create the source descriptor.
let seriesDescriptor =
HKQuantitySeriesSampleQueryDescriptor(predicate: predicate,
                                      options: .orderByQuantitySampleStartDate)

// Get the AsyncSequence that returns the individual data entries.
let series = seriesDescriptor.results(for: store)

// Access each data entry in the series
for try await entry in series {

    // Process results here.
    let steps = entry.quantity.doubleValue(for: .count())
    print(steps)
}
```

While this method returns an AsyncSequence, unlike the long-running queries, this sequence has a finite size. Iterating over the sequence asynchronously returns data entries, automatically terminating after you receive all the data.

## Topics

### Creating Series Query Descriptors

init(predicate: HKSamplePredicate&lt;HKQuantitySample>, options: HKQuantitySeriesSampleQueryDescriptor.Options)

Creates a quantity series query descriptor.

struct Options

Options used when querying series data.

### Running Queries

func results(for: HKHealthStore) -> HKQuantitySeriesSampleQueryDescriptor.Results

Runs a one-shot query that returns an asynchronous sequence of matching series samples.

struct Results

An asynchronous sequence that emits data from the quantity series query.

struct Result

A set of results from a quantity series sample descriptor.

### Accessing Query Properties

var options: HKQuantitySeriesSampleQueryDescriptor.Options

A set of options for the query. For a list of possible values, see HKQuantitySeriesSampleQueryDescriptor.Options.

var predicate: HKSamplePredicate&lt;HKQuantitySample>

A predicate that defines the set of series samples that the query returns.

### Default Implementations

HKAsyncSequenceQuery Implementations

## Relationships

### Conforms To

- Copyable
- HKAsyncSequenceQuery

## See Also

### Series queries

class HKQuantitySeriesSampleQuery

A query that accesses the series data associated with a quantity sample.

struct HKWorkoutRouteQueryDescriptor

A query interface that reads the location data stored in a workout route using Swift concurrency.

class HKWorkoutRouteQuery

A query to access the location data stored in a workout route.

struct HKHeartbeatSeriesQueryDescriptor

A query interface that reads the heartbeat series data stored in a heartbeat sample using Swift concurrency.

class HKHeartbeatSeriesQuery

A query that returns the heartbeat data contained in a heartbeat series sample.

struct HKElectrocardiogramQueryDescriptor

A query interface that reads the underlying voltage measurements for an electrocardiogram sample using Swift concurrency.

class HKElectrocardiogramQuery

A query that returns the underlying voltage measurements for an electrocardiogram sample.

