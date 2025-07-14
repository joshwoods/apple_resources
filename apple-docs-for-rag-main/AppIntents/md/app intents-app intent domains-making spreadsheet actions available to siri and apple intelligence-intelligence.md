

- App Intents
- App intent domains
-  Making spreadsheet actions available to Siri and Apple Intelligence 

Article

# Making spreadsheet actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s spreadsheet functionality with Siri and Apple Intelligence.

## Overview

To integrate your app’s spreadsheet capabilities with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent and app entity implementation that Apple Intelligence needs. For example, if your app allows someone to open a spreadsheet, use the AssistantIntent(schema:) macro and provide the assistant schema that consists of the `.spreadsheet` domain and the open schema:

```
@AssistantIntent(schema: .spreadsheet.open)
struct OpenSpreadsheetIntent: OpenIntent {
    var target: SpreadsheetDocumentEntity

    @MainActor
    func perform() async throws -> some IntentResult {
        return .result()
    }
}
```

To learn more about assistant schemas, see Integrating actions with Siri and Apple Intelligence. For a list of available app intents in the `.spreadsheet` domain, see AssistantSchemas.SpreadsheetIntent.

### Make sure your entity meets requirements

If you use app entities to describe custom data types, annotate the app entity implementation with the AssistantEntity(schema:) macro. This makes sure Siri and Apple Intelligence can understand your data. For example, the intent in the previous section uses `SpreadsheetEntity`. The following code snippet shows how the `SpreadsheetEntity` implementation uses the AssistantEntity(schema:) macro:

```
@AssistantEntity(schema: .spreadsheet.document)
struct SpreadsheetDocumentEntity {
    struct Query: EntityStringQuery {
        func entities(for identifiers: [SpreadsheetDocumentEntity.ID]) async throws -> [SpreadsheetDocumentEntity] { [] }
        func entities(matching string: String) async throws -> [SpreadsheetDocumentEntity] { [] }
    }

    static var defaultQuery = Query()
    var displayRepresentation: DisplayRepresentation { "Provide a display representation." }

    let id = UUID()

    var name: String
}
```

The assistant schema for the `PresentationEntity` consists of the `.spreadsheet` domain and the document schema.

For a list of available app entity schemas in the `.spreadsheet` domain, see AssistantSchemas.SpreadsheetEntity.

## See Also

### Spreadsheets

protocol SpreadsheetIntent

Assistant schema conformance for app intents that offer spreadsheet functionality.

protocol SpreadsheetEntity

Assistant schema conformance for app entities that describe spreadsheet data.

