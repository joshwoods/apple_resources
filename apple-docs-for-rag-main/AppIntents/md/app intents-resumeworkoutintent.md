

- App Intents
-  ResumeWorkoutIntent 

Protocol

# ResumeWorkoutIntent

An App Intent that lets someone resume your app’s paused workout session.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol ResumeWorkoutIntent : SystemIntent
```

## Mentioned in 

Responding to the Action button on Apple Watch Ultra

## Overview

On Apple Watch Ultra, someone can resume your app’s workout by simultaneously pressing the Action button and the side button when your app has a paused workout session.

To implement the resume action, create a structure that adopts the `ResumeWorkoutIntent` protocol.

```
struct MyResumeWorkoutIntent: ResumeWorkoutIntent {
    static var title: LocalizedStringResource = "Resume Workout"

    func perform() async throws -> some IntentResult {
        logger.debug("*** Performing a resume intent. ***")
        await MyWorkoutManager.shared.resumeWorkout()
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

protocol PauseWorkoutIntent

An App Intent that lets someone pause your app’s current workout session.

protocol StartDiveIntent

An App Intent that lets people start a dive session when they press the Action button on Apple Watch Ultra.

struct ConfirmationActionName

