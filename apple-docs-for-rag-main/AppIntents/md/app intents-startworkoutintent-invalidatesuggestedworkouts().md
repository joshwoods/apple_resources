

- App Intents
- StartWorkoutIntent
-  invalidateSuggestedWorkouts() 

Type Method

# invalidateSuggestedWorkouts()

Tells the system when the list of suggested workouts changes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func invalidateSuggestedWorkouts()
```

## Mentioned in 

Responding to the Action button on Apple Watch Ultra

## Discussion

Call this method when you change the value of the suggestedWorkouts property.

## See Also

### Defining supported workouts

associatedtype WorkoutStyle : AppValue

The type to use for defining the intent’s workout style.

**Required**

var workoutStyle: Self.WorkoutStyle

The workout style for the intent.

**Required**

static var suggestedWorkouts: [Self]

A list of the supported workout styles.

**Required**

