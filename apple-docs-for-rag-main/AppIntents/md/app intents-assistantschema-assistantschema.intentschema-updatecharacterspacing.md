

- App Intents
- AssistantSchema
- AssistantSchema.IntentSchema
-  updateCharacterSpacing 

Instance Property

# updateCharacterSpacing

The app intent conforms to the schema for updating the character spacing.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var updateCharacterSpacing: some AssistantSchemas.Intent { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent implementation.

For more information about the `.books` app intent domain, see Making ebook actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app intent that conforms to the `.books.updateCharacterSpacing` schema:

```
@AssistantIntent(schema: .books.updateCharacterSpacing)
struct UpdateCharacterSpacingIntent: AppIntent {
    @Parameter
    var target: BookSettingsEntity

    @Parameter
    var changeOperation: BookRelativeCharacterSpacingChange

    func perform() async throws -> some IntentResult {
        .result()
    }
}
```

