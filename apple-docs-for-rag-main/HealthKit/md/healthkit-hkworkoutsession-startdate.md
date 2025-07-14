

- HealthKit
- HKWorkoutSession
-  startDate 

Instance Property

# startDate

The starting time and date for this workout session.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 2.0+

``` source
var startDate: Date? { get }
```

## Discussion

This property is set to `nil` when the workout session is initialized. The system assigns a start date when the session’s state changes to HKWorkoutSessionState.running.

## See Also

### Accessing session data

var endDate: Date?

The ending time and date for this workout session.

var state: HKWorkoutSessionState

The workout session’s current state.

var type: HKWorkoutSessionType

A value that indicates whether the session is a primary session or a mirrored session.

var workoutConfiguration: HKWorkoutConfiguration

The configuration object that describes this workout.

