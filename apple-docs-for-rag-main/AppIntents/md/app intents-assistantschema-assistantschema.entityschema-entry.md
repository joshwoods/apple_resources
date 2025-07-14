

- App Intents
- AssistantSchema
- AssistantSchema.EntitySchema
-  entry 

Instance Property

# entry

The app entity describes a journal entry.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var entry: some AssistantSchemas.Entity { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app entity implementation.

For more information about the `.journal` app intent domain, see Making journaling actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app entity that conforms to the `.journal.entry` schema:

```
@AssistantEntity(schema: .journal.entry)
struct JournalEntity: AppEntity {
    struct Query: EntityStringQuery {
        func entities(for identifiers: [JournalEntity.ID]) async throws -> [JournalEntity] { [] }
        func entities(matching string: String) async throws -> [JournalEntity] { [] }
    }

    static var defaultQuery = Query()
    var displayRepresentation: DisplayRepresentation { "Journal Entry" }

    let id = UUID()

    @Property
    var title: String?

    @Property
    var message: AttributedString?

    @Property
    var mediaItems: [IntentFile]

    @Property
    var entryDate: Date?

    @Property
    var location: CLPlacemark?
}
```

