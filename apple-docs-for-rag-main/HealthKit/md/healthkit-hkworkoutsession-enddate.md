

- HealthKit
- HKWorkoutSession
-  endDate 

Instance Property

# endDate

The ending time and date for this workout session.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 2.0+

``` source
var endDate: Date? { get }
```

## Discussion

This property is set to `nil` when the workout session is initialized. The system assigns an end date when the session’s state changes to HKWorkoutSessionState.ended.

## See Also

### Accessing session data

var startDate: Date?

The starting time and date for this workout session.

var state: HKWorkoutSessionState

The workout session’s current state.

var type: HKWorkoutSessionType

A value that indicates whether the session is a primary session or a mirrored session.

var workoutConfiguration: HKWorkoutConfiguration

The configuration object that describes this workout.

