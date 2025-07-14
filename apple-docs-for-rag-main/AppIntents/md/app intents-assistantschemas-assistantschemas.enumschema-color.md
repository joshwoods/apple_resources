

- App Intents
- AssistantSchemas
- AssistantSchemas.EnumSchema
-  color 

Instance Property

# color

The color of a whiteboard canvas.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var color: some AssistantSchemas.Enum { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app enum implementation.

For more information about the `.whiteboard` app intent domain, see Making whiteboard actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app enum that conforms to the `.whiteboard.color` schema:

```
@AssistantEnum(schema: .whiteboard.color)
enum CanvasColor: AppEnum {
    case red
    case blue

    static var caseDisplayRepresentations: [CanvasColor: AppIntents.DisplayRepresentation] = [
        .red: "Red",
        .blue: "Blue",
    ]
}
```

