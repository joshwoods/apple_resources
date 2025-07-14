

- App Intents
- AssistantSchemas
- AssistantSchemas.EntitySchema
-  document 

Instance Property

# document

The app entity describes a text document.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var document: some AssistantSchemas.Entity { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app entity implementation.

For more information about the `.wordProcessor` app intent domain, see Making word processor actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app entity that conforms to the `.wordProcessor.document` schema:

```
@AssistantEntity(schema: .wordProcessor.document)
struct WordProcessorDocumentEntity: AppEntity {
    struct Query: EntityStringQuery {
        func entities(for identifiers: [WordProcessorDocumentEntity.ID]) async throws -> [WordProcessorDocumentEntity] { [] }
        func entities(matching string: String) async throws -> [WordProcessorDocumentEntity] { [] }
    }

    static var defaultQuery = Query()
    var displayRepresentation: DisplayRepresentation { "Text Document" }

    let id = UUID()

    @Property
    var name: String

    @Property
    var creationDate: Date?

    @Property
    var modificationDate: Date?
}
```

