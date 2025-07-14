

- App Intents
-  PauseWorkoutIntent 

Protocol

# PauseWorkoutIntent

An App Intent that lets someone pause your app’s current workout session.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol PauseWorkoutIntent : SystemIntent
```

## Mentioned in 

Responding to the Action button on Apple Watch Ultra

## Overview

On Apple Watch Ultra, someone can pause your workout by simultaneously pressing the Action button and the side button while your app is running a workout session.

To implement the pause action, create a structure that adopts the `PauseWorkoutIntent` protocol.

```
struct MyPauseWorkoutIntent: PauseWorkoutIntent {
   static var title: LocalizedStringResource = "Pause Workout"

   func perform() async throws -> some IntentResult {
       logger.debug("*** Performing a pause intent. ***")
       await MyWorkoutManager.shared.pauseWorkout()
       return .result()
   }
}
```

This intent needs a title property that provides a localized description of the action, and a perform() method, which the system calls when it triggers the intent.

For more information, see Responding to the Action button on Apple Watch Ultra.

## Relationships

### Inherits From

- AppIntent
- PersistentlyIdentifiable
- Sendable
- SystemIntent

## See Also

### Responding to the Action button

Responding to the Action button on Apple Watch Ultra

Use App Intents to register actions for your app.

protocol StartWorkoutIntent

An App Intent for starting a workout.

protocol ResumeWorkoutIntent

An App Intent that lets someone resume your app’s paused workout session.

protocol StartDiveIntent

An App Intent that lets people start a dive session when they press the Action button on Apple Watch Ultra.

struct ConfirmationActionName

