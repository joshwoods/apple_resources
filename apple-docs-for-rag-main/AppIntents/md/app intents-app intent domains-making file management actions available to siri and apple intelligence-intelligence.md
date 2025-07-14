

- App Intents
- App intent domains
-  Making file management actions available to Siri and Apple Intelligence 

Article

# Making file management actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s file management functionality with Siri and Apple Intelligence.

## Overview

To integrate your app’s file management functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent and app entity implementation that Apple Intelligence needs. For example, if your app allows a person to open a file, use the AssistantIntent(schema:) macro and provide the assistant schema that consists of the `.files` domain and the openFile schema:

```
@AssistantIntent(schema: .files.openFile)
struct OpenFileIntent: OpenIntent {
    var target: FileEntity

   func perform() async throws -> some IntentResult {
        return .result()
    }
}
```

To learn more about assistant schemas, see Integrating actions with Siri and Apple Intelligence. For a list of available app intents in the `.files` domain, see AssistantSchemas.FilesIntent.

### Make sure your entity meets requirements

If you use app entities to describe custom data types, annotate the app entity implementation with the AssistantEntity(schema:) macro. This makes sure Siri and Apple Intelligence can understand your data. For example, the intent in the previous section uses `FileEntity`. The following code snippet shows how the `FileEntity` implementation uses the AssistantEntity(schema:) macro:

```
@AssistantEntity(schema: .files.file)
struct FilesEntity: FileEntity {
    struct Query: EntityStringQuery {
        func entities(for identifiers: [FilesEntity.ID]) async throws -> [FilesEntity] { [] }
        func entities(matching string: String) async throws -> [FilesEntity] { [] }
    }
    static var defaultQuery = Query()

    static var supportedContentTypes = [UTType.image]
    var displayRepresentation: AppIntents.DisplayRepresentation { "Provide a display representation." }

    var id: FileEntityIdentifier

    var creationDate: Date?
    var fileModificationDate: Date?
}
```

The assistant schema for the `FileEntity` consists of the `.files` domain and the file schema.

For a list of available app entity schemas in the `.files` domain, see AssistantSchemas.FilesEntity.

## See Also

### File management

protocol FilesIntent

Assistant schema conformance for app intents that offer file management functionality.

protocol FilesEntity

Assistant schema conformance for app entities that describe files.

