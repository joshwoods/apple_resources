

- WorkoutKit
- PacerWorkout
-  supportsActivity(\_:) 

Type Method

# supportsActivity(\_:)

Returns a Boolean value that indicates whether the system supports pacer workouts for the given workout activity type.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
static func supportsActivity(_ activity: HKWorkoutActivityType) -> Bool
```

## Parameters 

`activity`  

The target workout activity type.

## See Also

### Creating a new pacer workout

init(activity: HKWorkoutActivityType, location: HKWorkoutSessionLocationType, distance: Measurement&lt;UnitLength>, time: Measurement&lt;UnitDuration>)

Creates a new pacer workout for the specified distance and time.

