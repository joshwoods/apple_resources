

- App Intents
- AssistantSchema
- AssistantSchema.IntentSchema
-  search 

Instance Property

# search

The app intent conforms to the schema for searching an ebook or audiobook library.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var search: some AssistantSchemas.Intent { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent implementation.

For more information about the `.books` app intent domain, see Making ebook actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app intent that conforms to the `.books.search` schema:

```
@AssistantIntent(schema: .books.search)
struct SearchLibraryIntent: ShowInAppSearchResultsIntent {
    @Parameter
    var criteria: StringSearchCriteria

    func perform() async throws -> some IntentResult {
        .result()
    }
}
```

