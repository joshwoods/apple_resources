

- HealthKit
-  HKHeartbeatSeriesQueryDescriptor 

Structure

# HKHeartbeatSeriesQueryDescriptor

A query interface that reads the heartbeat series data stored in a heartbeat sample using Swift concurrency.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct HKHeartbeatSeriesQueryDescriptor
```

## Overview

Use HKHeartbeatSeriesQueryDescriptor to read the heartbeat data included in a HKHeartbeatSeriesSample. To read the individual heartbeats, create a heartbeat series query descriptor using the desired series sample, and then call the results(for:) method on the descriptor.

```
// Create the descriptor.
let heartbeatDescriptor = HKHeartbeatSeriesQueryDescriptor(myHeartbeatSample)

// Get the AsyncSequence that returns individual heartbeats.
let series = heartbeatDescriptor.results(for: store)

// Access the data for each haeartbeat.
for try await heartbeat in series {

    // Process the results here.
    print(heartbeat.precededByGap)
    print(heartbeat.timeIntervalSinceStart)
}
```

While this method returns an AsyncSequence, unlike the long-running queries, this sequence has a finite size. Iterating over the sequence asynchronously returns heartbeat data, automatically terminating after you receive all the data.

## Topics

### Creating Heartbeat Series Query Descriptors

init(HKHeartbeatSeriesSample)

Creates a heartbeat series query descriptor.

### Running Queries

func results(for: HKHealthStore) -> HKHeartbeatSeriesQueryDescriptor.Results

Runs a one-shot query that returns an asynchronous sequence of data representing individual heartbeats.

struct Results

An asynchronous sequence that emits data about individual heartbeats from a heartbeat series sample.

struct Heartbeat

Data about an individual heartbeat.

### Accessing Query Properties

var sample: HKHeartbeatSeriesSample

The sample containing the heartbeat series.

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

class HKHeartbeatSeriesQuery

A query that returns the heartbeat data contained in a heartbeat series sample.

struct HKElectrocardiogramQueryDescriptor

A query interface that reads the underlying voltage measurements for an electrocardiogram sample using Swift concurrency.

class HKElectrocardiogramQuery

A query that returns the underlying voltage measurements for an electrocardiogram sample.

