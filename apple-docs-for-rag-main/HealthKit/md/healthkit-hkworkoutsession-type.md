

- HealthKit
- HKWorkoutSession
-  type 

Instance Property

# type

A value that indicates whether the session is a primary session or a mirrored session.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 10.0+

``` source
var type: HKWorkoutSessionType { get }
```

## See Also

### Accessing session data

var endDate: Date?

The ending time and date for this workout session.

var startDate: Date?

The starting time and date for this workout session.

var state: HKWorkoutSessionState

The workout session’s current state.

var workoutConfiguration: HKWorkoutConfiguration

The configuration object that describes this workout.

