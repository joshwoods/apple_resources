

- App Intents
- StartWorkoutIntent
-  suggestedWorkouts 

Type Property

# suggestedWorkouts

A list of the supported workout styles.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var suggestedWorkouts: [Self] { get }
```

**Required**

## Mentioned in 

Responding to the Action button on Apple Watch Ultra

## Discussion

If your app is installed on Apple Watch Ultra, the system displays these workouts as options under the First Press settings when someone sets your app as the workout app in Settings \> Action Button.

For a complete description of implementing a StartWorkoutIntent, see Responding to the Action button on Apple Watch Ultra

## See Also

### Defining supported workouts

associatedtype WorkoutStyle : AppValue

The type to use for defining the intent’s workout style.

**Required**

var workoutStyle: Self.WorkoutStyle

The workout style for the intent.

**Required**

static func invalidateSuggestedWorkouts()

Tells the system when the list of suggested workouts changes.

