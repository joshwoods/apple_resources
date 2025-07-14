

- App Intents
- AssistantSchema
- AssistantSchema.IntentSchema
-  openDocument 

Instance Property

# openDocument

The app intent conforms to the schema for opening a text document.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var openDocument: some AssistantSchemas.Intent { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent implementation.

For more information about the `.reader` app intent domain, see Making document reader actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app intent that conforms to the `.reader.openDocument` schema:

```
@AssistantIntent(schema: .reader.openDocument)
struct ReaderOpenDocumentsIntent: AppIntent {
    @Parameter
    var files: [IntentFile]

    func perform() async throws -> some IntentResult {
        return .result()
    }
}
```

