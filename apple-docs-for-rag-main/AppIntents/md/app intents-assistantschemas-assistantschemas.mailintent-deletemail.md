

- App Intents
- AssistantSchemas
- AssistantSchemas.MailIntent
-  deleteMail 

Instance Property

# deleteMail

The app intent conforms to the schema for deleting email messages.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var deleteMail: some AssistantSchemas.Intent { get }
```

## Overview

To integrate your app’s functionality with Siri and Apple Intelligence, you use Swift macros that generate additional properties and add protocol conformance for your app intent implementation.

For more information about the `.mail` app intent domain, see Making email actions available to Siri and Apple Intelligence. For general information about app intent domains, see Integrating actions with Siri and Apple Intelligence.

The following example shows an app intent that conforms to the `.mail.deleteMail` schema:

```
@AssistantIntent(schema: .mail.deleteMail)
struct DeleteMailIntent: DeleteIntent {
    @Parameter
    var entities: [MailMessageEntity]

    func perform() async throws -> some IntentResult {
        .result()
    }
}
```

