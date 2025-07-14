

- App Intents
- App intent domains
-  Making word processor actions available to Siri and Apple Intelligence 

Article

# Making word processor actions available to Siri and Apple Intelligence

Create app intents and entities that make your app’s word processor functionality available to Siri and Apple Intelligence.

## Overview

To integrate your app’s word processor capabilities with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent and app entity implementation that Apple Intelligence needs. For example, if your app allows someone to open a text document, use the AssistantIntent(schema:) macro and provide the assistant schema that consists of the `.wordProcessor` domain and the open schema:

```
@AssistantIntent(schema: .wordProcessor.open)
struct OpenWordProcessorDocumentIntent: OpenIntent {
    var target: WordProcessorDocumentEntity

    func perform() async throws -> some IntentResult {
        .result()
    }
}
```

To learn more about assistant schemas, see Integrating actions with Siri and Apple Intelligence. For a list of available app intents in the `.wordProcessor` domain, see AssistantSchemas.WordProcessorIntent.

### Make sure your entity meets requirements

If you use app entities to describe custom data types, annotate the app entity implementation with the AssistantEntity(schema:) macro. This makes sure Siri and Apple Intelligence can understand your data. For example, the intent in the previous section uses `DocumentEntity`. The following code snippet shows how the `DocumentEntity` implementation uses the AssistantEntity(schema:) macro:

```
@AssistantEntity(schema: .wordProcessor.document)
struct WordProcessorDocumentEntity {
    struct Query: EntityStringQuery {
        func entities(for identifiers: [WordProcessorDocumentEntity.ID]) async throws -> [WordProcessorDocumentEntity] { [] }
        func entities(matching string: String) async throws -> [WordProcessorDocumentEntity] { [] }
    }

    static var defaultQuery = Query()
    var displayRepresentation: DisplayRepresentation { "Provide a display representation." }

    let id = UUID()

    var name: String
    var creationDate: Date?
    var modificationDate: Date?
}
```

The assistant schema for the `DocumentEntity` consists of the `.wordProcessor` domain and the document schema.

For a list of available app entity schemas in the `.wordProcessor` domain, see AssistantSchemas.WordProcessorEntity.

## See Also

### Word processor and text editing

protocol WordProcessorIntent

Assistant schema conformance for app intents that offer word processing functionality.

protocol WordProcessorEntity

Assistant schema conformance for app entities that describe text documents.

