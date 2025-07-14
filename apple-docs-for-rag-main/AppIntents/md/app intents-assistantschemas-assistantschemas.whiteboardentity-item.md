

- App Intents
- AssistantSchemas
- AssistantSchemas.WhiteboardEntity
-  item 

Instance Property

# item

The app entity describes an item on a whiteboard canvas.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var item: some AssistantSchemas.Entity { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app entity implementation.

For more information about the `.whiteboard` app intent domain, see Making whiteboard actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app entity that conforms to the `.whiteboard.item` schema:

```
@AssistantEntity(schema: .whiteboard.item)
struct CanvasItemEntity: AppEntity {
    struct Query: EntityStringQuery {
        func entities(for identifiers: [CanvasItemEntity.ID]) async throws -> [CanvasItemEntity] { [] }
        func entities(matching string: String) async throws -> [CanvasItemEntity] { [] }
    }

    static var defaultQuery = Query()
    var displayRepresentation: DisplayRepresentation { "Canvas Item" }

    let id = UUID()

    @Property
    var type: CanvasItemType

    @Property
    var label: String?

    @Property
    var x: Double

    @Property
    var y: Double

    @Property
    var width: Double?

    @Property
    var height: Double?
}
```

