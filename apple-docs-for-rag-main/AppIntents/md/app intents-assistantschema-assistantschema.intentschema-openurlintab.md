

- App Intents
- AssistantSchema
- AssistantSchema.IntentSchema
-  openURLInTab 

Instance Property

# openURLInTab

The app intent conforms to the Assistant schema for loading a URL in a browser tab.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var openURLInTab: some AssistantSchemas.Intent { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent implementation.

For more information about the `.browser` app intent domain, see Making browser actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app intent that conforms to the `.browser.openURLInTab` schema:

```
@AssistantIntent(schema: .browser.openURLInTab)
struct LoadURLInTabIntent: AppIntent {
    @Parameter
    var tab: TabEntity

    @Parameter
    var url: URL

    func perform() async throws -> some IntentResult {
        .result()
    }
}
```

