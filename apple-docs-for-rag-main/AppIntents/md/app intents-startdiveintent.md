

- App Intents
-  StartDiveIntent 

Protocol

# StartDiveIntent

An App Intent that lets people start a dive session when they press the Action button on Apple Watch Ultra.

watchOS 9.0+

``` source
protocol StartDiveIntent : SystemIntent
```

## Mentioned in 

Responding to the Action button on Apple Watch Ultra

## Overview

To implement the start dive action, create a structure that adopts the `StartDiveIntent` protocol.

```
struct MyStartDiveIntent: StartDiveIntent {

    static var title: LocalizedStringResource = "Starting a dive session."

    func perform() async throws -> some IntentResult {
        logger.debug("*** Starting a dive session. ***")

        await DiveManager.shared.start()
        return .result(actionButtonIntent: StartDive())
    }
}
```

This intent needs a title property that provides a localized description of the action, and a perform() method, which the system calls when it triggers the intent.

To read live depth, water pressure, and water temperature data, see Accessing submersion data.

Important

Before you can access live dive data, your app needs to include an entitlement to access submersion data. For more information, see Express interest in the Submerged Depth and Pressure API.

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

protocol ResumeWorkoutIntent

An App Intent that lets someone resume your app’s paused workout session.

struct ConfirmationActionName

