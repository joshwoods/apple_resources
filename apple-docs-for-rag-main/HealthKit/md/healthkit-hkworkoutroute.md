

- HealthKit
-  HKWorkoutRoute 

Class

# HKWorkoutRoute

A sample that contains a workout’s route data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
class HKWorkoutRoute
```

## Mentioned in 

Reading route data

Creating a workout route

## Overview

When creating a workout route, you do not instantiate the HKWorkoutRoute objects directly. Instead, create a HKWorkoutRouteBuilder object, and provide it with location data throughout the workout. After the workout ends, call the route builder’s finishRoute(with:metadata:completion:) method to create the route. For detailed instructions, see Creating a workout route.

The route’s location data is stored as an array of CLLocation objects. Because the route may contain a large number of location objects, use a HKWorkoutRouteQuery object to asynchronously read the location data from the HealthKit store in batches. For more information, see Reading route data.

### Using workout routes

Like many HealthKit classes, the HKWorkoutRoute class should not be subclassed. You can extend HKWorkoutRoute objects by adding custom metadata keys and values to the metadata dictionary when the object is created.

## Relationships

### Inherits From

- HKSeriesSample

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Route data

Creating a workout route

Record the user’s route during a workout.

Reading route data

Access the user’s route for a workout.

class HKWorkoutRouteBuilder

A builder object that incrementally constructs a workout route.

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

