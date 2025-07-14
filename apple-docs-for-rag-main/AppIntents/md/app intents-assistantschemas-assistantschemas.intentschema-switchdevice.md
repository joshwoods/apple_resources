

- App Intents
- AssistantSchemas
- AssistantSchemas.IntentSchema
-  switchDevice 

Instance Property

# switchDevice

The app intent conforms to the schema for switching between cameras or devices.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var switchDevice: some AssistantSchemas.Intent { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent implementation.

For more information about the `.camera` app intent domain, see Making camera actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app intent that conforms to the `.camera.switchDevice` schema:

```
@AssistantIntent(schema: .camera.switchDevice)
struct FlipCameraIntent: AppIntent {

    func perform() async throws -> some IntentResult {
        .result()
    }
}
```

