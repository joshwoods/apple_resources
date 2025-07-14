

- App Intents
- AssistantSchemas
- AssistantSchemas.WhiteboardIntent
-  createItem 

Instance Property

# createItem

The app intent conforms to the schema for creating an item on a whiteboard canvas.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var createItem: some AssistantSchemas.Intent { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent implementation.

For more information about the `.whiteboard` app intent domain, see Making whiteboard actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app intent that conforms to the `.whiteboard.createItem` schema:

```
@AssistantIntent(schema: .whiteboard.createItem)
struct CreateCanvasItemIntent: AppIntent {
    @Parameter
    var target: CanvasEntity

    @Parameter
    var itemType: CanvasItemType?

    @Parameter
    var text: String?

    @Parameter
    var mediaItems: [IntentFile]

    @Parameter
    var url: URL?

    func perform() async throws -> some ReturnsValue {
        .result(value: CanvasItemEntity())
    }
}
```

