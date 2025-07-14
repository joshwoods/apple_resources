

- App Intents
- AssistantSchemas
- AssistantSchemas.WordProcessorIntent
-  addWebVideoToPage 

Instance Property

# addWebVideoToPage

The app intent conforms to the schema for adding a web video to a page in a text document.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var addWebVideoToPage: some AssistantSchemas.Intent { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent implementation.

For more information about the `.wordProcessor` app intent domain, see Making word processor actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app intent that conforms to the `.wordProcessor.addWebVideoToPage` schema:

```
@AssistantIntent(schema: .wordProcessor.addWebVideoToPage)
struct AddWebVideoToWordProcessorPageIntent: AppIntent {
    @Parameter
    var target: WordProcessorPageEntity

    @Parameter(supportedContentTypes: [.audio])
    var audio: IntentFile

    func perform() async throws -> some IntentResult {
        .result()
    }
}
```

