

- HealthKit
-  HKSeriesSample 

Class

# HKSeriesSample

An abstract base class that defines samples that contain a series of items.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
class HKSeriesSample
```

## Overview

Never instantiate HKSeriesSample objects directly. Instead, user one of the concrete subclasses (for example, the HKWorkoutRoute class).

## Topics

### Accessing the series

var count: Int

The number of items in the series.

## Relationships

### Inherits From

- HKSample

### Inherited By

- HKHeartbeatSeriesSample
- HKWorkoutRoute

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

