

- App Intents
- AssistantSchema
- AssistantSchema.EntitySchema
-  book 

Instance Property

# book

The app entity describes an ebook.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var book: some AssistantSchemas.Entity { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app entity implementation.

For more information about the `.books` app intent domain, see Making ebook actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app entity that conforms to the `.books.book` schema:

```
@AssistantEntity(schema: .books.book)
struct BookEntity: AppEntity {
    struct Query: EntityStringQuery {
        func entities(for identifiers: [BookEntity.ID]) async throws -> [BookEntity] { [] }
        func entities(matching string: String) async throws -> [BookEntity] { [] }
    }

    static var defaultQuery = Query()
    var displayRepresentation: DisplayRepresentation { "Book" }

    let id = UUID()

    @Property
    var title: String?

    @Property
    var seriesTitle: String?

    @Property
    var author: String?

    @Property
    var genre: String?

    @Property
    var purchaseDate: Date?

    @Property
    var contentType: BookContentType?
}
```

