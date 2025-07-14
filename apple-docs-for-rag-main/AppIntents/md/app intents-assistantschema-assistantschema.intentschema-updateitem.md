

- App Intents
- AssistantSchema
- AssistantSchema.IntentSchema
-  updateItem 

Instance Property

# updateItem

The app intent conforms to the schema for updating an item on a whiteboard canvas.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var updateItem: some AssistantSchemas.Intent { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent implementation.

For more information about the `.whiteboard` app intent domain, see Making whiteboard actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app intent that conforms to the `.whiteboard.updateItem` schema:

```
@AssistantIntent(schema: .whiteboard.updateItem)
struct UpdateCanvasItemIntent: AppIntent {
    @Parameter
    var target: CanvasItemEntity

    @Parameter
    var color: CanvasColor?

    @Parameter
    var label: String?

    func perform() async throws -> some IntentResult {
        .result()
    }
}
```

