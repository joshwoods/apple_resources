

- HealthKit
-  HKElectrocardiogramQueryDescriptor 

Structure

# HKElectrocardiogramQueryDescriptor

A query interface that reads the underlying voltage measurements for an electrocardiogram sample using Swift concurrency.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct HKElectrocardiogramQueryDescriptor
```

## Overview

Use HKElectrocardiogramQueryDescriptor to access the individual voltage measurements associated with an HKElectrocardiogram sample. To read the individual voltage measurements, create an electrocardiogram query descriptor using the desired sample, and then call the results(for:) method on the descriptor.

```
// Create the descriptor.
let ecgDescriptor = HKElectrocardiogramQueryDescriptor(myElectrocardiogram)

// Get the AsyncSequence that returns individual voltage measurements.
let voltages = ecgDescriptor.results(for: store)

// Access each voltage measurement.
for try await measurement in voltages {

    // Process the results here.
    print(measurement.quantity(for: .appleWatchSimilarToLeadI) ?? "No Measurement")
    print(measurement.timeSinceSampleStart)
}
```

While this method returns an AsyncSequence, unlike the long-running queries, this sequence has a finite size. Iterating over the sequence asynchronously returns voltage measurements, automatically terminating after you receive all the measurements.

## Topics

### Creating Electrocardiogram Query Descriptors

init(HKElectrocardiogram)

Creates a query descriptor that reads voltage measurements from the provided electrocardiogram sample.

### Running Queries

func results(for: HKHealthStore) -> HKElectrocardiogramQueryDescriptor.Results

Runs a one-shot query that returns an asynchronous sequence of data representing individual heartbeats.

struct Results

An asynchronous sequence that emits data about individual voltage measurements from an electrocardiogram sample.

### Accessing Query Properties

var electrocardiogram: HKElectrocardiogram

The sample that contains the voltage measurements.

### Default Implementations

HKAsyncSequenceQuery Implementations

## Relationships

### Conforms To

- Copyable
- HKAsyncSequenceQuery

## See Also

### Series queries

struct HKQuantitySeriesSampleQueryDescriptor

A query interface that reads the series data associated with quantity samples using Swift concurrency.

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

class HKElectrocardiogramQuery

A query that returns the underlying voltage measurements for an electrocardiogram sample.

