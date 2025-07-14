

- HealthKit
-  HKWorkoutRouteQueryDescriptor 

Structure

# HKWorkoutRouteQueryDescriptor

A query interface that reads the location data stored in a workout route using Swift concurrency.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
struct HKWorkoutRouteQueryDescriptor
```

## Overview

Use HKWorkoutRouteQueryDescriptor to access the individual CLLocation objects stored in an HKWorkoutRoute sample. To read the individual locations, create a workout route query descriptor using the desired route, and then call the descriptor’s results(for:) method.

```
// Create the descriptor.
let routeQueryDescriptor = HKWorkoutRouteQueryDescriptor(myRoute)

// Get the AsyncSequence that returns individual locations.
let locations = routeQueryDescriptor.results(for: store)

// Access each location.
for try await location in locations {

    // Process the results here.
    print(location.coordinate)
    print(location.timestamp)
}
```

While this method returns an AsyncSequence, unlike the long-running queries, this sequence has a finite size. Iterating over the sequence asynchronously returns the route’s locations, automatically terminating after you receive all the locations.

## Topics

### Creating workout route query descriptors

init(HKWorkoutRoute)

Creates a query descriptor that reads locations from the provided workout route sample.

### Running queries

func results(for: HKHealthStore) -> HKWorkoutRouteQueryDescriptor.Results

Runs a one-shot query that returns an asynchronous sequence of data representing individual locations.

struct Results

An asynchronous sequence that emits data about individual locations from a workout route sample.

### Accessing query properties

var workoutRoute: HKWorkoutRoute

A workout route sample that contains locations.

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

