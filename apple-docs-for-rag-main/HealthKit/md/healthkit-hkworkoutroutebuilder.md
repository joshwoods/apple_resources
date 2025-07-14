

- HealthKit
-  HKWorkoutRouteBuilder 

Class

# HKWorkoutRouteBuilder

A builder object that incrementally constructs a workout route.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
class HKWorkoutRouteBuilder
```

## Overview

To create a workout route, instantiate a HKWorkoutRouteBuilder, and provide it with location data throughout the workout. After the workout ends, call the builder’s finishRoute(with:metadata:completion:) method to construct the route. For detailed instructions, see `Creating a Workout Route`.

## Topics

### Creating the builder

init(healthStore: HKHealthStore, device: HKDevice?)

Creates and returns a new workout route builder.

### Building the route

func finishRoute(with: HKWorkout, metadata: [String : Any]?, completion: (HKWorkoutRoute?, (any Error)?) -> Void)

Creates, saves, and associates the route with the provided workout.

func insertRouteData([CLLocation], completion: (Bool, (any Error)?) -> Void)

Adds route data to the builder.

func addMetadata([String : Any], completion: (Bool, (any Error)?) -> Void)

Adds metadata to the builder.

## Relationships

### Inherits From

- HKSeriesBuilder

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Route data

Creating a workout route

Record the user’s route during a workout.

Reading route data

Access the user’s route for a workout.

class HKWorkoutRoute

A sample that contains a workout’s route data.

struct HKWorkoutRouteQueryDescriptor

A query interface that reads the location data stored in a workout route using Swift concurrency.

class HKWorkoutRouteQuery

A query to access the location data stored in a workout route.

let HKWorkoutRouteTypeIdentifier: String

A series sample containing location data that defines the route the user took during a workout.

class HKSeriesBuilder

An abstract base class for building series samples.

class HKSeriesSample

An abstract base class that defines samples that contain a series of items.

