

- App Intents
- App intent domains
-  Making journaling actions available to Siri and Apple Intelligence 

Article

# Making journaling actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s journaling functionality with Siri and Apple Intelligence.

## Overview

To integrate your app’s journaling capabilities with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent and app entity implementation that Apple Intelligence needs. For example, if your app allows someone to create a new journal entry, use the AssistantIntent(schema:) macro and provide the assistant schema that consists of the `.journal` domain and the createEntry schema:

```
@AssistantIntent(schema: .journal.createEntry)
struct CreateJournalEntryIntent {
    var message: AttributedString
    var title: String?
    var entryDate: Date?
    var location: CLPlacemark?

    @Parameter(default: [])
    var mediaItems: [IntentFile]

    func perform() async throws -> some ReturnsValue {
        .result(value: JournalEntryEntity)
    }
}

```

To learn more about assistant schemas, see Integrating actions with Siri and Apple Intelligence. For a list of available app intents in the `.journal` domain, see AssistantSchemas.JournalIntent.

### Make sure your entity meets requirements

If you use app entities to describe custom data types, annotate the app entity implementation with the AssistantEntity(schema:) macro. This makes sure Siri and Apple Intelligence can understand your data. For example, the intent in the previous section uses `JournalEntity`. The following code snippet shows how the `JournalEntity` implementation uses the AssistantEntity(schema:) macro:

```
@AssistantEntity(schema: .journal.entry)
struct JournalEntryEntity {
    struct Query: EntityStringQuery {
        func entities(for identifiers: [JournalEntryEntity.ID]) async throws -> [JournalEntryEntity] { [] }
        func entities(matching string: String) async throws -> [JournalEntryEntity] { [] }
    }

    static var defaultQuery = Query()
    var displayRepresentation: DisplayRepresentation { "Provide a display representation." }

    let id = UUID()

    var title: String?
    var message: AttributedString?
    var mediaItems: [IntentFile]
    var entryDate: Date?
    var location: CLPlacemark?
}
```

The assistant schema for the `JournalEntity` consists of the `.journal` domain and the entry schema.

For a list of available app entity schemas in the `.journal` domain, see AssistantSchemas.JournalEntity.

## See Also

### Journaling

protocol JournalIntent

Assistant schema conformance for app intents that offer journaling functionality.

protocol JournalEntity

Assistant schema conformance for app entities that describe journaling data.

