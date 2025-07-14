

- App Intents
- App intent domains
-  Making in-app search actions available to Siri and Apple Intelligence 

Article

# Making in-app search actions available to Siri and Apple Intelligence

Create app intents and entities to integrate your app’s search functionality with Siri and Apple Intelligence.

## Overview

To integrate your in-app search with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance to your ShowInAppSearchResultsIntent implementation. Use the AssistantIntent(schema:) macro and provide the assistant schema that consists of the `.system` domain and the search schema:

```
import AppIntents
import Foundation

@AssistantIntent(schema: .system.search)
struct ExampleSearchIntent: ShowInAppSearchResultsIntent {
    static var searchScopes: [StringSearchScope] = [.general]
    var criteria: StringSearchCriteria

    func perform() async throws -> some IntentResult {
        let searchString = criteria.term
        print("Searching for \(searchString)")
        // ...
        // Code that navigates to your app's search and enters the search string into a search field.
        // ...
        return .result()
    }
}
```

To learn more about assistant schemas, see Integrating actions with Siri and Apple Intelligence.

## See Also

### System and in-app search

protocol SystemIntent

Assistant schema conformance for app intents that match system-provided intents.

