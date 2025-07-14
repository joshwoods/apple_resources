

- HealthKit
- HKWorkoutSession
-  workoutConfiguration 

Instance Property

# workoutConfiguration

The configuration object that describes this workout.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var workoutConfiguration: HKWorkoutConfiguration { get }
```

## Discussion

Returns a copy of the configuration object passed to init(configuration:) when instantiating the workout session. Changes made to the returned value have no affect on the workout session.

## See Also

### Accessing session data

var endDate: Date?

The ending time and date for this workout session.

var startDate: Date?

The starting time and date for this workout session.

var state: HKWorkoutSessionState

The workout session’s current state.

var type: HKWorkoutSessionType

A value that indicates whether the session is a primary session or a mirrored session.

