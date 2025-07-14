

- HealthKit
- HKWorkoutSession
-  currentActivity 

Instance Property

# currentActivity

The current workout activity.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 9.0+

``` source
@NSCopying
var currentActivity: HKWorkoutActivity { get }
```

## Discussion

This property contains a workout activity that’s currently in progress (an activity with an endDate property set to `nil`). If you end the activity — for example, by calling endCurrentActivity(on:) or updateActivity(uuid:end:completion:) — the system sets this property to `nil` until you begin a new activity.

## See Also

### Managing workout activities

func beginNewActivity(configuration: HKWorkoutConfiguration, date: Date, metadata: [String : Any]?)

Begins a new workout activity in the workout session.

func endCurrentActivity(on: Date)

Ends the current workout activity.

