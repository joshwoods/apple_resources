

- HealthKit
-  HKLiveWorkoutDataSource 

Class

# HKLiveWorkoutDataSource

A data source that automatically provides live data from an active workout session.

macOSwatchOS 5.0+

``` source
class HKLiveWorkoutDataSource
```

## Mentioned in 

Running workout sessions

## Topics

### Creating a live data source

init(healthStore: HKHealthStore, workoutConfiguration: HKWorkoutConfiguration?)

Creates a new data source based on the provided workout configuration.

var typesToCollect: Set&lt;HKQuantityType>

The quantity type samples that the data source automatically sends to the workout builder.

### Calculating statistics

func enableCollection(for: HKQuantityType, predicate: NSPredicate?)

Begins automatically calculating statistics for samples that match the quantity type and predicate.

func disableCollection(for: HKQuantityType)

Stops automatically calculating statistics for the quantity type.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Sessions

Running workout sessions

Track a workout on Apple Watch.

Build a workout app for Apple Watch

Create your own workout app, quickly and easily, with HealthKit and SwiftUI.

Building a multidevice workout app

Mirror a workout from a watchOS app to its companion iOS app, and perform bidirectional communication between them.

class HKWorkoutSession

A session that tracks the user’s workout on Apple Watch.

class HKWorkoutConfiguration

An object that contains configuration information about a workout session.

enum HKWorkoutSessionState

A workout session’s state.

class HKLiveWorkoutBuilder

A builder object that constructs a workout incrementally based on live data from an active workout session.

