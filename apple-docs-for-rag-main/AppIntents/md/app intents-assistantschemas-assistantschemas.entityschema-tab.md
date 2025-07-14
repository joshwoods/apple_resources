

- App Intents
- AssistantSchemas
- AssistantSchemas.EntitySchema
-  tab 

Instance Property

# tab

The app entity describes a browser tab.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var tab: some AssistantSchemas.Entity { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app entity implementation.

For more information about the `.browser` app intent domain, see Making browser actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app entity that conforms to the `.browser.tab` schema:

```
@AssistantEntity(schema: .browser.tab)
struct TabEntity: AppEntity {
    static var defaultQuery = Query()

    let id = UUID()

    @Property
    var url: URL?

    @Property
    var name: String

    @Property
    var isPrivate: Bool

    var displayRepresentation: AppIntents.DisplayRepresentation { "Tab" }
    struct Query: EntityStringQuery {
        func entities(for identifiers: [TabEntity.ID]) async throws -> [TabEntity] { [] }
        func entities(matching string: String) async throws -> [TabEntity] { [] }
    }
}
```

