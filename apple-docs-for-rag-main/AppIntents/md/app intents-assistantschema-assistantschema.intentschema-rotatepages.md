

- App Intents
- AssistantSchema
- AssistantSchema.IntentSchema
-  rotatePages 

Instance Property

# rotatePages

The app intent conforms to the schema for rotating a page.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var rotatePages: some AssistantSchemas.Intent { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent implementation.

For more information about the `.reader` app intent domain, see Making document reader actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app intent that conforms to the `.reader.rotatePages` schema:

```
@AssistantIntent(schema: .reader.rotatePages)
struct ReaderRotatePagesIntent: AppIntent {
    @Parameter
    var pages: [ReaderPageEntity]

    @Parameter
    var isClockwise: Bool

    func perform() async throws -> some IntentResult & ReturnsValue {
        return .result(value: [ReaderPageEntity()])
    }
}
```

