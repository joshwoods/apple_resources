

- App Intents
- AssistantSchema
- AssistantSchema.EntitySchema
-  recognizedPerson 

Instance Property

# recognizedPerson

The app entity describes a person who appears in an asset.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var recognizedPerson: some AssistantSchemas.Entity { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app entity implementation.

For more information about the `.photos` app intent domain, see Making photo and video actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app entity that conforms to the `.photos.recognizedPerson` schema:

```
@AssistantEntity(schema: .photos.recognizedPerson)
struct PhotoPersonEntity: AppEntity {
    struct Query: EntityStringQuery {
        func entities(for identifiers: [PhotoPersonEntity.ID]) async throws -> [PhotoPersonEntity] { [] }
        func entities(matching string: String) async throws -> [PhotoPersonEntity] { [] }
    }

    static var defaultQuery = Query()
    var displayRepresentation: DisplayRepresentation { "Photo Person" }

    let id = UUID()

    @Property
    var name: String

    @Property
    var isFavorite: Bool
}
```

