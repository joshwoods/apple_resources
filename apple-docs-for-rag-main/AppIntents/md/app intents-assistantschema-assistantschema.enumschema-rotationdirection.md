

- App Intents
- AssistantSchema
- AssistantSchema.EnumSchema
-  rotationDirection 

Instance Property

# rotationDirection

The direction for rotating a photo or video.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var rotationDirection: some AssistantSchemas.Enum { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app enum implementation.

For more information about the `.photos` app intent domain, see Making photo and video actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app enum that conforms to the `.photos.rotationDirection` schema:

```
@AssistantEnum(schema: .photos.rotationDirection)
enum PhotoRotationDirection: AppEnum {
    case clockwise

    static var caseDisplayRepresentations: [PhotoRotationDirection: AppIntents.DisplayRepresentation] = [
        .clockwise: "Clockwise",
    ]
}
```

