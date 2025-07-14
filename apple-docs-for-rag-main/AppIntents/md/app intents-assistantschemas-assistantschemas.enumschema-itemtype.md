

- App Intents
- AssistantSchemas
- AssistantSchemas.EnumSchema
-  itemType 

Instance Property

# itemType

The type of an item on a whiteboard canvas.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var itemType: some AssistantSchemas.Enum { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app enum implementation.

For more information about the `.whiteboard` app intent domain, see Making whiteboard actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app enum that conforms to the `.whiteboard.itemType` schema:

```
@AssistantEnum(schema: .whiteboard.itemType)
enum CanvasItemType: AppEnum {
    case square
    case circle

    static var caseDisplayRepresentations: [CanvasItemType: AppIntents.DisplayRepresentation] = [
        .square: "Square",
        .circle: "Circle",
    ]
}
```

