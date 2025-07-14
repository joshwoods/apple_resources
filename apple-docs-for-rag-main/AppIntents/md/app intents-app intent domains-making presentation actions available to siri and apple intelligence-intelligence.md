

- App Intents
- App intent domains
-  Making presentation actions available to Siri and Apple Intelligence 

Article

# Making presentation actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s presentation functionality with Siri and Apple Intelligence.

## Overview

To integrate your app’s presentation capabilities with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent and app entity implementation that Apple Intelligence needs. For example, if your app allows someone to open a presentation, use the AssistantIntent(schema:) macro and provide the assistant schema that consists of the `.presentation` domain and the createSlide schema:

```
@AssistantIntent(schema: .presentation.open)
struct OpenPresentationIntent: OpenIntent {
    var target: PresentationEntity

    func perform() async throws -> some IntentResult {
        .result()
    }
}
```

To learn more about assistant schemas, see Integrating actions with Siri and Apple Intelligence. For a list of available app intents in the `.presentation` domain, see AssistantSchemas.PresentationIntent.

### Make sure your entity meets requirements

If you use app entities to describe custom data types, annotate the app entity implementation with the AssistantEntity(schema:) macro. This makes sure Siri and Apple Intelligence can understand your data. For example, the intent in the previous section uses `PresentationEntity`. The following code snippet shows how the `PresentationEntity` implementation uses the AssistantEntity(schema:) macro:

```
@AssistantEntity(schema: .presentation.document)
struct PresentationEntity {
    struct Query: EntityStringQuery {
        func entities(for identifiers: [PresentationEntity.ID]) async throws -> [PresentationEntity] { [] }
        func entities(matching string: String) async throws -> [PresentationEntity] { [] }
    }

    static var defaultQuery = Query()
    var displayRepresentation: DisplayRepresentation { "Provide a display representation." }

    let id = UUID()

    var name: String
}
```

The assistant schema for the `PresentationEntity` consists of the `.presentation` domain and the document schema.

For a list of available app entity schemas in the `.presentation` domain, see AssistantSchemas.PresentationEntity.

## See Also

### Presentations

protocol PresentationIntent

Assistant schema conformance for app intents that offer presentation functionality.

protocol PresentationEntity

Assistant schema conformance for app entities that describe presentation data.

