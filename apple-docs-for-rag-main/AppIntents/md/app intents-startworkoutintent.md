

- App Intents
-  StartWorkoutIntent 

Protocol

# StartWorkoutIntent

An App Intent for starting a workout.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol StartWorkoutIntent : InstanceDisplayRepresentable, SystemIntent
```

## Mentioned in 

Responding to the Action button on Apple Watch Ultra

## Overview

On Apple Watch Ultra, this intent registers a start workout action for the Action button. After installing your app, the user can select this action in Settings \> Action Button by setting Action to Workout and App to your app.

When implementing this intent, define the following:

- A title property

- A workoutStyle property

- A list of suggestedWorkouts

- A displayRepresentation property

- A perform() method

```
struct MyStartWorkoutIntent: StartWorkoutIntent {

    // Define the intent's title.
    static var title: LocalizedStringResource = "Start Workout"

    // Define a list of start workout intents that appear below the First Press
    // settings when someone sets your app as the workout app in
    // Settings > Action Button.
    static var suggestedWorkouts: [MyStartWorkoutIntent] = [MyStartWorkoutIntent()]

    // Define a parameter that specifies the type of workout that this
    // intent starts.
    @Parameter(title: "Start Workout Entity")
    var workoutStyle: WorkoutEnum

    // Define an init method that sets the default workout type.
    init() {
        workoutStyle = .workout
    }

    // Set the display representation based on the current workout style.
    var displayRepresentation: DisplayRepresentation {
        WorkoutEnum.caseDisplayRepresentations[workoutStyle] ??
        DisplayRepresentation(title: "Unknown")
    }

    // Launch your app when the system triggers this intent.
    static var openAppWhenRun: Bool { true }

    // Define the method that the system calls when it triggers this event.
    func perform() async throws -> some IntentResult {
        let workoutManager = MyWorkoutManager.shared
        await workoutManager.requestAuthorization()
        await workoutManager.startWorkout()
        return .result()
    }
}
```

Important

When defining the workoutStyle property, ensure that it adopts either the AppEnum or AppEntity protocol. Declare this property using the AppIntent.Parameter property wrapper.

For more information, see Responding to the Action button on Apple Watch Ultra.

## Topics

### Creating an intent

init(style: Self.WorkoutStyle)

Creates a new intent for the specified workout style.

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

static func invalidateSuggestedWorkouts()

Tells the system when the list of suggested workouts changes.

## Relationships

### Inherits From

- AppIntent
- CustomLocalizedStringResourceConvertible
- InstanceDisplayRepresentable
- PersistentlyIdentifiable
- Sendable
- SystemIntent

## See Also

### Responding to the Action button

Responding to the Action button on Apple Watch Ultra

Use App Intents to register actions for your app.

protocol PauseWorkoutIntent

An App Intent that lets someone pause your app’s current workout session.

protocol ResumeWorkoutIntent

An App Intent that lets someone resume your app’s paused workout session.

protocol StartDiveIntent

An App Intent that lets people start a dive session when they press the Action button on Apple Watch Ultra.

struct ConfirmationActionName

