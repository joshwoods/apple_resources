

- App Intents
- StartWorkoutIntent
-  workoutStyle 

Instance Property

# workoutStyle

The workout style for the intent.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var workoutStyle: Self.WorkoutStyle { get set }
```

**Required**

## Mentioned in 

Responding to the Action button on Apple Watch Ultra

## Discussion

Your implementation’s `workoutStyle` property must be a type you define that adopts either the AppEnum or AppEntity protocol. Declare this property using the AppIntent.Parameter property wrapper.

```
// Define a parameter that specifies the type of workout that this
// intent starts.
@Parameter(title: "Start Workout Entity")
var workoutStyle: WorkoutEnum
```

For a complete description of implementing a StartWorkoutIntent, see Responding to the Action button on Apple Watch Ultra

## See Also

### Defining supported workouts

associatedtype WorkoutStyle : AppValue

The type to use for defining the intent’s workout style.

**Required**

static var suggestedWorkouts: [Self]

A list of the supported workout styles.

**Required**

static func invalidateSuggestedWorkouts()

Tells the system when the list of suggested workouts changes.

