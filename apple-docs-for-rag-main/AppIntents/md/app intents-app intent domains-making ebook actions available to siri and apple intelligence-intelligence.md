

- App Intents
- App intent domains
-  Making ebook actions available to Siri and Apple Intelligence 

Article

# Making ebook actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s ebook and audiobook functionality with Siri and Apple Intelligence.

## Overview

To integrate your app’s ebook and audiobook capabilities with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent, app entity, and app enumeration implementation that Apple Intelligence needs. For example, if your app allows a person to open an ebook, use the AssistantIntent(schema:) macro and provide the assistant schema that consists of the `.books` domain and the openBook schema:

```
@AssistantIntent(schema: .books.openBook)
struct OpenBookIntent: OpenIntent {
    var target: BookEntity

    func perform() async throws -> some IntentResult {
        .result()
    }
}
```

To learn more about assistant schemas, see Integrating actions with Siri and Apple Intelligence. For a list of available app intents in the `.books` domain, see AssistantSchemas.BooksIntent.

### Make sure your entity meets requirements

If you use app entities to describe custom data types, annotate the app entity implementation with the AssistantEntity(schema:) macro. This makes sure Siri and Apple Intelligence can understand your data. For example, the intent in the previous section uses `BookEntity`. The following code snippet shows how the `BookEntity` implementation uses the AssistantEntity(schema:) macro:

```
@AssistantEntity(schema: .books.book)
struct BookEntity {
    struct Query: EntityStringQuery {
        func entities(for identifiers: [BookEntity.ID]) async throws -> [BookEntity] { [] }
        func entities(matching string: String) async throws -> [BookEntity] { [] }
    }

    static var defaultQuery = Query()
    var displayRepresentation: DisplayRepresentation { "Provide a display representation." }

    let id = UUID()

    var title: String?
    var seriesTitle: String?
    var author: String?
    var genre: String?
    var purchaseDate: Date?
    var contentType: BookContentType?
    var url: URL?
}
```

The assistant schema for the `BookEntity` consists of the `.books` domain and the book schema.

For a list of available app entity schemas in the `.books` domain, see AssistantSchemas.BooksEntity.

### Make sure your enumeration meets requirements

To make sure Siri and Apple Intelligence understand custom static types for your intent parameters, annotate app enumerations with the AssistantEnum(schema:) macro. Then, pass the `.books` domain and a schema to it. The following example uses the contentType schema:

```
@AssistantEnum(schema: .books.contentType)
enum BookContentType: String, AppEnum {
    case book
    case pdf

    static var caseDisplayRepresentations: [BookContentType: AppIntents.DisplayRepresentation] = [:]

}
```

For a list of available app enumeration schemas in the `.books` domain, see AssistantSchemas.BooksEnum.

## See Also

### Books

protocol BooksIntent

Assistant schema conformance for app intents that offer ebook and audiobook functionality.

protocol BooksEntity

Assistant schema conformance for app entities that describe ebooks or audiobooks.

protocol BooksEnum

Assistant schema conformance for types you use to describe ebooks or audiobooks.

