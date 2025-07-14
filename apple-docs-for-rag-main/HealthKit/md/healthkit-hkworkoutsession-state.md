

- HealthKit
- HKWorkoutSession
-  state 

Instance Property

# state

The workout session’s current state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 2.0+

``` source
var state: HKWorkoutSessionState { get }
```

## Discussion

For a list of possible session states, see HKWorkoutSessionState.

## See Also

### Accessing session data

var endDate: Date?

The ending time and date for this workout session.

var startDate: Date?

The starting time and date for this workout session.

var type: HKWorkoutSessionType

A value that indicates whether the session is a primary session or a mirrored session.

var workoutConfiguration: HKWorkoutConfiguration

The configuration object that describes this workout.

