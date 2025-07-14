

- App Intents
- AssistantSchemas
- AssistantSchemas.EnumSchema
-  captureMode 

Instance Property

# captureMode

The capture mode for taking a photo or video.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var captureMode: some AssistantSchemas.Enum { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app enum implementation.

For more information about the `.camera` app intent domain, see Making camera actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app enum that conforms to the `.camera.captureMode` schema:

```
@AssistantEnum(schema: .camera.captureMode)
enum CaptureMode: AppEnum {
    case selfie
    case video

    static var caseDisplayRepresentations: [CaptureMode: AppIntents.DisplayRepresentation] = [
        .selfie: "Selfie",
        .video: "Video",
    ]
}
```

