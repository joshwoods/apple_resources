

- App Intents
- AssistantSchemas
- AssistantSchemas.IntentSchema
-  addTextBoxToSlide 

Instance Property

# addTextBoxToSlide

The app intent conforms to the schema for adding a text box to a slide.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var addTextBoxToSlide: some AssistantSchemas.Intent { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent implementation.

For more information about the `.presentation` app intent domain, see Making presentation actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app intent that conforms to the `.presentation.addTextBoxToSlide` schema:

```
@AssistantIntent(schema: .presentation.addTextBoxToSlide)
struct AddTextBoxToPresentationSlideIntent: AppIntent {
    @Parameter
    var target: PresentationSlideEntity

    @Parameter
    var text: String

    func perform() async throws -> some IntentResult {
        .result()
    }
}
```

