

- App Intents
- AssistantSchemas
- AssistantSchemas.PresentationEntity
-  document 

Instance Property

# document

The app entity describes a presentation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var document: some AssistantSchemas.Entity { get }
```

## Mentioned in 

Making presentation actions available to Siri and Apple Intelligence

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app entity implementation.

For more information about the `.presentation` app intent domain, see Making presentation actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app entity that conforms to the `.presentation.document` schema:

```
@AssistantEntity(schema: .presentation.document)
struct PresentationEntity: AppEntity {
    struct Query: EntityStringQuery {
        func entities(for identifiers: [PresentationEntity.ID]) async throws -> [PresentationEntity] { [] }
        func entities(matching string: String) async throws -> [PresentationEntity] { [] }
    }

    static var defaultQuery = Query()
    var displayRepresentation: DisplayRepresentation { "Presentation" }

    let id = UUID()

    @Property
    var name: String
}
```

