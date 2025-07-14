

- App Intents
- AssistantSchemas
- AssistantSchemas.BrowserEntity
-  window 

Instance Property

# window

The app entity describes a browser window.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var window: some AssistantSchemas.Entity { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app entity implementation.

For more information about the `.browser` app intent domain, see Making browser actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app entity that conforms to the `.browser.window` schema:

```
@AssistantEntity(schema: .browser.window)
struct WindowEntity: AppEntity {
    static var defaultQuery = Query()

    let id = UUID()

    @Property
    var tabs: [TabEntity]

    @Property
    var isPrivate: Bool

    var displayRepresentation: AppIntents.DisplayRepresentation { "Window" }
    struct Query: EntityStringQuery {
        func entities(for identifiers: [WindowEntity.ID]) async throws -> [WindowEntity] { [] }
        func entities(matching string: String) async throws -> [WindowEntity] { [] }
    }
}
```

