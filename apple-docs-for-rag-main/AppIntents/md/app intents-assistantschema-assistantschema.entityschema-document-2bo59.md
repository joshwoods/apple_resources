

- App Intents
- AssistantSchema
- AssistantSchema.EntitySchema
-  document 

Instance Property

# document

The app entity describes a spreadsheet.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var document: some AssistantSchemas.Entity { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app entity implementation.

For more information about the `.spreadsheet` app intent domain, see Making spreadsheet actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app entity that conforms to the `.spreadsheet.document` schema:

```
@AssistantEntity(schema: .spreadsheet.document)
struct SpreadsheetEntity: AppEntity {
    struct Query: EntityStringQuery {
        func entities(for identifiers: [SpreadsheetEntity.ID]) async throws -> [SpreadsheetEntity] { [] }
        func entities(matching string: String) async throws -> [SpreadsheetEntity] { [] }
    }

    static var defaultQuery = Query()
    var displayRepresentation: DisplayRepresentation { "Spreadsheet" }

    let id = UUID()

    @Property
    var name: String

}
```

