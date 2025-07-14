

- App Intents
- App intent domains
-  Making whiteboard actions available to Siri and Apple Intelligence 

Article

# Making whiteboard actions available to Siri and Apple Intelligence

Create app intents and entities that make your app’s whiteboard functionality available to Siri and Apple Intelligence.

## Overview

To integrate your app’s whiteboard capabilities with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent and app entity implementation that Apple Intelligence needs. For example, if your app allows someone to open a whiteboard, use the AssistantIntent(schema:) macro and provide the assistant schema that consists of the `.whiteboard` domain and the createBoard schema:

```
@AssistantIntent(schema: .whiteboard.createBoard)
struct CreateWhiteboardIntent: AppIntent {
    public var title: String?

    func perform() async throws -> some ReturnsValue {
        .result(value: WhiteboardBoardEntity())
    }
}
```

To learn more about assistant schemas, see Integrating actions with Siri and Apple Intelligence. For a list of available app intents in the `.whiteboard` domain, see AssistantSchemas.WhiteboardIntent.

### Make sure your entity meets requirements

If you use app entities to describe custom data types, annotate the app entity implementation with the AssistantEntity(schema:) macro. This makes sure Siri and Apple Intelligence can understand your data. For example, the intent in the previous section uses `WhiteboardEntity`. The following code snippet shows how the `WhiteboardEntity` implementation uses the AssistantEntity(schema:) macro:

```
@AssistantEntity(schema: .whiteboard.board)
struct WhiteboardBoardEntity {
    struct Query: EntityStringQuery {
        func entities(for identifiers: [WhiteboardBoardEntity.ID]) async throws -> [WhiteboardBoardEntity] { [] }
        func entities(matching string: String) async throws -> [WhiteboardBoardEntity] { [] }
    }

    static var defaultQuery = Query()
    var displayRepresentation: DisplayRepresentation { "Provide a display representation." }

    let id = UUID()

    var title: String
    var creationDate: Date
    var lastModificationDate: Date
}
```

The assistant schema for the `WhiteboardBoardEntity` consists of the `.whiteboard` domain and the board schema.

For a list of available app entity schemas in the `.whiteboard` domain, see AssistantSchemas.WhiteboardEntity.

### Make sure your enumeration meets requirements

To make sure Siri and Apple Intelligence understand custom static types for your intent parameters, annotate app enumerations with the AssistantEnum(schema:) macro. Then, pass the `.whiteboard` domain and a schema to it. The following example uses the color schema:

```
@AssistantEnum(schema: .whiteboard.color)
enum WhiteboardColor: String, AppEnum {
    case white
    case black
    case grey
    case green
    case red
    case blue
    case yourCustomAppColor

    static var caseDisplayRepresentations: [WhiteboardColor: AppIntents.DisplayRepresentation] = [:]

}
```

For a list of available app enums in the `.whiteboard` domain, refer to AssistantSchemas.WhiteboardEnum.

## See Also

### Whiteboard

protocol WhiteboardIntent

Assistant schema conformance for app intents that offer whiteboard functionality.

protocol WhiteboardEntity

Assistant schema conformance for app entities that describe data for whiteboard functionality.

protocol WhiteboardEnum

Assistant schema conformance for whiteboard types.

